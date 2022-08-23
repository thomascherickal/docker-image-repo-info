<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.15`](#julia1-alpine315)
-	[`julia:1-alpine3.16`](#julia1-alpine316)
-	[`julia:1-bullseye`](#julia1-bullseye)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-windowsservercore`](#julia1-windowsservercore)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2022`](#julia1-windowsservercore-ltsc2022)
-	[`julia:1.6`](#julia16)
-	[`julia:1.6-alpine`](#julia16-alpine)
-	[`julia:1.6-alpine3.15`](#julia16-alpine315)
-	[`julia:1.6-alpine3.16`](#julia16-alpine316)
-	[`julia:1.6-bullseye`](#julia16-bullseye)
-	[`julia:1.6-buster`](#julia16-buster)
-	[`julia:1.6-windowsservercore`](#julia16-windowsservercore)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2022`](#julia16-windowsservercore-ltsc2022)
-	[`julia:1.6.7`](#julia167)
-	[`julia:1.6.7-alpine`](#julia167-alpine)
-	[`julia:1.6.7-alpine3.15`](#julia167-alpine315)
-	[`julia:1.6.7-alpine3.16`](#julia167-alpine316)
-	[`julia:1.6.7-bullseye`](#julia167-bullseye)
-	[`julia:1.6.7-buster`](#julia167-buster)
-	[`julia:1.6.7-windowsservercore`](#julia167-windowsservercore)
-	[`julia:1.6.7-windowsservercore-1809`](#julia167-windowsservercore-1809)
-	[`julia:1.6.7-windowsservercore-ltsc2022`](#julia167-windowsservercore-ltsc2022)
-	[`julia:1.8`](#julia18)
-	[`julia:1.8-alpine`](#julia18-alpine)
-	[`julia:1.8-alpine3.15`](#julia18-alpine315)
-	[`julia:1.8-alpine3.16`](#julia18-alpine316)
-	[`julia:1.8-bullseye`](#julia18-bullseye)
-	[`julia:1.8-buster`](#julia18-buster)
-	[`julia:1.8-windowsservercore`](#julia18-windowsservercore)
-	[`julia:1.8-windowsservercore-1809`](#julia18-windowsservercore-1809)
-	[`julia:1.8-windowsservercore-ltsc2022`](#julia18-windowsservercore-ltsc2022)
-	[`julia:1.8.0`](#julia180)
-	[`julia:1.8.0-alpine`](#julia180-alpine)
-	[`julia:1.8.0-alpine3.15`](#julia180-alpine315)
-	[`julia:1.8.0-alpine3.16`](#julia180-alpine316)
-	[`julia:1.8.0-bullseye`](#julia180-bullseye)
-	[`julia:1.8.0-buster`](#julia180-buster)
-	[`julia:1.8.0-windowsservercore`](#julia180-windowsservercore)
-	[`julia:1.8.0-windowsservercore-1809`](#julia180-windowsservercore-1809)
-	[`julia:1.8.0-windowsservercore-ltsc2022`](#julia180-windowsservercore-ltsc2022)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.15`](#juliaalpine315)
-	[`julia:alpine3.16`](#juliaalpine316)
-	[`julia:bullseye`](#juliabullseye)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore`](#juliawindowsservercore)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2022`](#juliawindowsservercore-ltsc2022)

## `julia:1`

```console
$ docker pull julia@sha256:f063fdefb5a45ab75f3309c6e0a43f691a4100def0ae20caa233c74b26632bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.15`

```console
$ docker pull julia@sha256:31b5056cbbd8f8af176d7ea40d7417ba6601e19c77858c8f0d3ced6a368e5002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:b7845cc320f6103c310ee765472bd55e09d7996a0844ccb932fbd85693faf26f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151954583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0757795c13b54d40903e67e7860639c8c4ed667060a620c7fa02ecbd0bfb610d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:50 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:30:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:30:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db51d58571ac8192edc30a955119ab6d5a7c2d8a2c8604f2a94708be1eeeaec`  
		Last Modified: Fri, 19 Aug 2022 00:33:17 GMT  
		Size: 149.1 MB (149131071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.16`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-bullseye`

```console
$ docker pull julia@sha256:43a3661152a3366a0be3694bf955d8b3cc8cfa765b7199bc90a4cbe46c2967fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:7caf803419e4a454079f5b009a3097af34be08e8b47585d5d1e3af576e4f4b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:640642febd41f81d62607f5ce24fdca0e39b2060bcb3c56d49de52eb5603a903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179293925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef8073afa115ed02ab45dfa57b701ff85499d98010c3181a654267115db0ce2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:34:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1964a73f39838efa7af98609a61ecf1ba3266086831790ee3de7c71c0e6ec711`  
		Last Modified: Tue, 23 Aug 2022 03:36:23 GMT  
		Size: 4.5 MB (4468185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a104f3aff5ce20a6849b1477f4099735247ccfb1367958f9c488e5f40045fdd7`  
		Last Modified: Tue, 23 Aug 2022 03:36:45 GMT  
		Size: 147.7 MB (147687410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5eb5e78a2a9d028e17c0b5a07698e2337e532c7b4e7c5cbdcacef2769d7a9e05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171538865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3439f7910be37bb39acd736a62737601fc7c5730f34adc9e8a6967c12003bde9`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:28:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:28:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:28:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:10 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:28:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee5ef9658b8af75e5d8cbd34d5a919e156f9da0588ac3a3b1501cd9b6a98081`  
		Last Modified: Tue, 23 Aug 2022 04:30:31 GMT  
		Size: 4.3 MB (4346922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9958c3807c3314e6e599a4904ff947f31c08c358635ab79d9de63ab80f838b4f`  
		Last Modified: Tue, 23 Aug 2022 04:30:51 GMT  
		Size: 141.3 MB (141279428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:d3ff6e52e422c4a0c78857deb1482f85c49ea045b6e4377555caa28e1548962e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176958712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94b068ddad4812a4c890228329edecdcd8be47afd6066284340d46d33d5ee5`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:07 GMT
ADD file:69e3a870d6821a7b0d69402e3d7bc6488f1ed7d86dc5cf7f5f35d5868b72eaf3 in / 
# Tue, 23 Aug 2022 01:03:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:52:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:52:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:52:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:25 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:46d42afa0260ad958104e1c87669868156eb23042a5c897146b1d7009ac682d9`  
		Last Modified: Tue, 23 Aug 2022 01:09:21 GMT  
		Size: 27.8 MB (27797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564ab79e374248c2778afffda8f2aa8a38a3c6e7d60c75426e41b9773387e20`  
		Last Modified: Tue, 23 Aug 2022 11:54:52 GMT  
		Size: 4.6 MB (4616209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c3b90157dbe01d07e902812add81f9d5607811adfd3e387d19bad31225a3c0`  
		Last Modified: Tue, 23 Aug 2022 11:55:10 GMT  
		Size: 144.5 MB (144544818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore`

```console
$ docker pull julia@sha256:aeaeacee9115fb97e300dadcba1ce584f70785a9010cfbf2ba6ab8d2b67a23d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:bb2ec07816d9c5d0bd9f326119a53882a494cb038e2a6cdcd4a832720fd002b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:d456bc1037ec50a9558c1143a8dfb6712820851fae28aa4773ce45ddeb8d40e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:1-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:473c2adb82d0b9a9852f59aa6b16ef40e8b7f1b73aa61a611cc3369217e1fd6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:a33ccdfc660d2fbb36d7b811416e8c329a519935c685ea2b78e4649ee3fd6992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156447962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baf29e645cdf3ea1843317e4dd205abdd46a9517e333764f52efe46d1e4666`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:31 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 03:34:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c6af71d41cbf7d55043019d8a9c2af7620996a44311776c725591431fdcdad`  
		Last Modified: Tue, 23 Aug 2022 03:37:22 GMT  
		Size: 122.6 MB (122639906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:23b46a7eed27310efd6ccc0b57e52e3094e7b084584194fb56dee6f553a233e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142488195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91f738fbe5e6176a15d2ce1eb6ec56393a9d47849c7838dc27d727268406033`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:00:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 18:00:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 18:00:52 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 18:01:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 18:01:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dd18e755cf320ec3c4a92559bb88648650871437863819346dff6c089befdd`  
		Last Modified: Tue, 23 Aug 2022 18:02:25 GMT  
		Size: 2.2 MB (2228774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f43c56ceb161c543292679ef861fe2bc6853a9f251d27cd5974ee6a0ebdaaa`  
		Last Modified: Tue, 23 Aug 2022 18:02:50 GMT  
		Size: 113.7 MB (113687689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:68ea505e8fc7975a8d22c4e4835f94ce4b19909642a2181f67a276c2e9e858db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148486570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc694b41b0dd18ed24140dd69bdd3340f0ecf746a24d626189e5f65eba5fdb6f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:32 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 04:28:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541cfdbd8d7dec8e159c1286d13d5d1abd6942c6b02cca72986ce5693d2f1d2`  
		Last Modified: Tue, 23 Aug 2022 04:31:26 GMT  
		Size: 116.2 MB (116213278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:950b6532cf73ad077690e2088e27d1e9c15f2317a24ddbcc934ffca29385aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aefceeb9932d832416b48f44d01edacba83095c583ac6a220f6a96e34b05672`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:51 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 11:53:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:53:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879c19315299064e3c73e34f5ee1c2abfbb8ab802ecd12456385998dbc228765`  
		Last Modified: Tue, 23 Aug 2022 11:55:42 GMT  
		Size: 120.1 MB (120090724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:a0818af2e0f8a13d4222356885970a613ec3b8610f0acafbda07ec20106981c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2451579016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e044ab27d86c37c4edaf9a01364962ee26df9b81fb003e4366acdb77f77413`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:18:30 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:18:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:18:32 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:19:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27460b61e7e0840b17c8d59299b4932215a5271d962024858263938f3140370b`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65d1a9c24024a1c33f1fd0e611f1b8dea64e66de1f9d448ef8b750f76c15bf`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006990ee1247492ce82d3a7c72562b9737e20b40d5b6c4c59264919bf3b48ed`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e610c6a735851c58863c1aa77010c7bfe7adeed65c34a96d12a60416f281d8`  
		Last Modified: Wed, 10 Aug 2022 15:26:09 GMT  
		Size: 134.7 MB (134683215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09da6580b4ce486d7a85b080bd0c32e5d645fdbfd95baa002c9a7de58ed2c93c`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:a569e4731001467b267880dcc8d4f47289bd869a2001c38ce6a89c17a0fd271d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2812127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89843c1f4ebe099a51e15c435efc21eade6e4638066610f1626a910c6b6db878`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:19:57 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:19:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:19:59 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:21:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:21:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3530803da63720880f09e29040253e0f8fdebfb174978069f5b511d94216e`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02860751ea1196e0da1978bd80bdf7121b7e5769ff8713ca222c594035ff44`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fc1649eaa6b9174a6017d79b08ed23399aa70d3a40443f2b8843c1cdb65ba`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c032438917b21bcb582bd0cf1ef0ddcb31952a557601cd3cd347f4837c8dfa45`  
		Last Modified: Wed, 10 Aug 2022 15:26:47 GMT  
		Size: 134.4 MB (134407545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bac399186798527168b7633aec7516f048b4d5221c10e5fbbd41743fa767ff`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine`

```console
$ docker pull julia@sha256:abad5660f5a25b83328226f94c06f079ae52e1516c0964ca60425f8609470e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine` - linux; amd64

```console
$ docker pull julia@sha256:d3ce5d6d5d6f52656a02cf4c856bebd70b3bcbc03dcbe998dd8742fe6bc69a33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124634697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caf39300b6c77f62601cb1d00732814d855bb6adb601fcfaa30ee52fc91e391e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:44:03 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 09 Aug 2022 20:44:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:44:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f330082d37d521e85ed048135a49bb04735375b78ee4f62596d0fe91ddf609bd`  
		Last Modified: Tue, 09 Aug 2022 20:48:32 GMT  
		Size: 121.8 MB (121828643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.15`

```console
$ docker pull julia@sha256:3eaf1cf9731fbedfca9fc5ab8120a5f8168fd29ce23767061f64a02f6fb38091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:bbbffe7594e3fbb20aedd6c3ba81e9d5d327cd9f63728c7dbe809260d53d2ace
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124652106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b946aaf71e28d5eb07e343a7c2cee7b04d8ac744c4f1d362d64fd0e369931842`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:44:22 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 09 Aug 2022 20:44:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:44:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8ddc086b261016ce741f48368107159bdc66980c1f74a6324a65fc523cacb9`  
		Last Modified: Tue, 09 Aug 2022 20:49:06 GMT  
		Size: 121.8 MB (121828594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.16`

```console
$ docker pull julia@sha256:abad5660f5a25b83328226f94c06f079ae52e1516c0964ca60425f8609470e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:d3ce5d6d5d6f52656a02cf4c856bebd70b3bcbc03dcbe998dd8742fe6bc69a33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124634697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caf39300b6c77f62601cb1d00732814d855bb6adb601fcfaa30ee52fc91e391e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:44:03 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 09 Aug 2022 20:44:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:44:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f330082d37d521e85ed048135a49bb04735375b78ee4f62596d0fe91ddf609bd`  
		Last Modified: Tue, 09 Aug 2022 20:48:32 GMT  
		Size: 121.8 MB (121828643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-bullseye`

```console
$ docker pull julia@sha256:5d1506755eba77f8fde18de9fadaeaf12b259ab8a4782b0ef55569e30566fbf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:a33ccdfc660d2fbb36d7b811416e8c329a519935c685ea2b78e4649ee3fd6992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156447962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baf29e645cdf3ea1843317e4dd205abdd46a9517e333764f52efe46d1e4666`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:31 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 03:34:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c6af71d41cbf7d55043019d8a9c2af7620996a44311776c725591431fdcdad`  
		Last Modified: Tue, 23 Aug 2022 03:37:22 GMT  
		Size: 122.6 MB (122639906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:23b46a7eed27310efd6ccc0b57e52e3094e7b084584194fb56dee6f553a233e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142488195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91f738fbe5e6176a15d2ce1eb6ec56393a9d47849c7838dc27d727268406033`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:00:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 18:00:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 18:00:52 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 18:01:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 18:01:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dd18e755cf320ec3c4a92559bb88648650871437863819346dff6c089befdd`  
		Last Modified: Tue, 23 Aug 2022 18:02:25 GMT  
		Size: 2.2 MB (2228774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f43c56ceb161c543292679ef861fe2bc6853a9f251d27cd5974ee6a0ebdaaa`  
		Last Modified: Tue, 23 Aug 2022 18:02:50 GMT  
		Size: 113.7 MB (113687689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:68ea505e8fc7975a8d22c4e4835f94ce4b19909642a2181f67a276c2e9e858db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148486570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc694b41b0dd18ed24140dd69bdd3340f0ecf746a24d626189e5f65eba5fdb6f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:32 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 04:28:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541cfdbd8d7dec8e159c1286d13d5d1abd6942c6b02cca72986ce5693d2f1d2`  
		Last Modified: Tue, 23 Aug 2022 04:31:26 GMT  
		Size: 116.2 MB (116213278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; 386

```console
$ docker pull julia@sha256:950b6532cf73ad077690e2088e27d1e9c15f2317a24ddbcc934ffca29385aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aefceeb9932d832416b48f44d01edacba83095c583ac6a220f6a96e34b05672`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:51 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 11:53:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:53:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879c19315299064e3c73e34f5ee1c2abfbb8ab802ecd12456385998dbc228765`  
		Last Modified: Tue, 23 Aug 2022 11:55:42 GMT  
		Size: 120.1 MB (120090724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:ac755e4a7a7a8364d6826e97e7fc9c82f220f9edae2c856804bf7c98528f406f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:ea3d52b8f06a09466df00b7de874240f263987e691873f96ecf7b5a911a45e4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154256163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101468a6f4cb99683b7f2788e6efc2df637727617bdd8e75f9d2ac60881a5973`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:34:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:50 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 03:35:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:35:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1964a73f39838efa7af98609a61ecf1ba3266086831790ee3de7c71c0e6ec711`  
		Last Modified: Tue, 23 Aug 2022 03:36:23 GMT  
		Size: 4.5 MB (4468185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e68eedbd2e9810c460134ace2381bf4c9bcdd7417bf6f922adaf1df3244a24`  
		Last Modified: Tue, 23 Aug 2022 03:37:51 GMT  
		Size: 122.6 MB (122649648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:29c5995ecdaffa347784776196e245c183c22da081deb197be84cb73aa08ef78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140253760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d1a8e51f38053ffdfc1a96e2fa653d06b75b0b6dc9c42e4f5c96a836043a0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 18:01:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 18:01:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 18:01:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 18:01:36 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 18:01:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 18:01:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6db4cf3a1e061a4bf1b4b5edf5b2aa7a5a9ad2239595b233a737fd58306baa`  
		Last Modified: Tue, 23 Aug 2022 18:03:04 GMT  
		Size: 3.8 MB (3811306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcdf7854ddd3e52b07c0a65ec22aeda15c7e65b7d9c58ab60ef805e3a7ba98`  
		Last Modified: Tue, 23 Aug 2022 18:03:28 GMT  
		Size: 113.7 MB (113695756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:d7ad07d964dce0935bc1daf7156f2a20c61d60c9cc468c41afc0dec3c3497cf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146481680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:001bb81f0eedd2e4e4d565e3579ef6ff4b961c48fca1e93c595cdfa758b38888`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:28:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:28:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:28:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:59 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 04:29:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:29:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee5ef9658b8af75e5d8cbd34d5a919e156f9da0588ac3a3b1501cd9b6a98081`  
		Last Modified: Tue, 23 Aug 2022 04:30:31 GMT  
		Size: 4.3 MB (4346922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b454e73f1e6abff01d763a6279aecc024eaf7c134f68ec9568c03509969c079`  
		Last Modified: Tue, 23 Aug 2022 04:31:54 GMT  
		Size: 116.2 MB (116222243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:91073a6d07f316382b34a9a5841958626881b6e296eba0555f57c617ca85a08f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.5 MB (152517064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df444009e83271e4ba28d60eba568e233882430e1a9987684e2f2d349850ac80`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:07 GMT
ADD file:69e3a870d6821a7b0d69402e3d7bc6488f1ed7d86dc5cf7f5f35d5868b72eaf3 in / 
# Tue, 23 Aug 2022 01:03:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:52:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:52:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:52:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:53:15 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 11:53:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:53:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:46d42afa0260ad958104e1c87669868156eb23042a5c897146b1d7009ac682d9`  
		Last Modified: Tue, 23 Aug 2022 01:09:21 GMT  
		Size: 27.8 MB (27797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564ab79e374248c2778afffda8f2aa8a38a3c6e7d60c75426e41b9773387e20`  
		Last Modified: Tue, 23 Aug 2022 11:54:52 GMT  
		Size: 4.6 MB (4616209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbad84e0d169c9851168aa30b06b5c5eeb1fc007ef701390df4950677d592ecb`  
		Last Modified: Tue, 23 Aug 2022 11:56:10 GMT  
		Size: 120.1 MB (120103170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore`

```console
$ docker pull julia@sha256:8a4505711835e404073fd2c7295bd101f4ff396ef6afd77eb9b9d666b2dc16f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.6-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:a0818af2e0f8a13d4222356885970a613ec3b8610f0acafbda07ec20106981c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2451579016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e044ab27d86c37c4edaf9a01364962ee26df9b81fb003e4366acdb77f77413`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:18:30 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:18:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:18:32 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:19:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27460b61e7e0840b17c8d59299b4932215a5271d962024858263938f3140370b`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65d1a9c24024a1c33f1fd0e611f1b8dea64e66de1f9d448ef8b750f76c15bf`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006990ee1247492ce82d3a7c72562b9737e20b40d5b6c4c59264919bf3b48ed`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e610c6a735851c58863c1aa77010c7bfe7adeed65c34a96d12a60416f281d8`  
		Last Modified: Wed, 10 Aug 2022 15:26:09 GMT  
		Size: 134.7 MB (134683215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09da6580b4ce486d7a85b080bd0c32e5d645fdbfd95baa002c9a7de58ed2c93c`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:a569e4731001467b267880dcc8d4f47289bd869a2001c38ce6a89c17a0fd271d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2812127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89843c1f4ebe099a51e15c435efc21eade6e4638066610f1626a910c6b6db878`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:19:57 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:19:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:19:59 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:21:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:21:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3530803da63720880f09e29040253e0f8fdebfb174978069f5b511d94216e`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02860751ea1196e0da1978bd80bdf7121b7e5769ff8713ca222c594035ff44`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fc1649eaa6b9174a6017d79b08ed23399aa70d3a40443f2b8843c1cdb65ba`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c032438917b21bcb582bd0cf1ef0ddcb31952a557601cd3cd347f4837c8dfa45`  
		Last Modified: Wed, 10 Aug 2022 15:26:47 GMT  
		Size: 134.4 MB (134407545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bac399186798527168b7633aec7516f048b4d5221c10e5fbbd41743fa767ff`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:a1f71101fad9124c34869394fb7ae1032fa4d5267a33752c9b76d61731a62c66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:a569e4731001467b267880dcc8d4f47289bd869a2001c38ce6a89c17a0fd271d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2812127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89843c1f4ebe099a51e15c435efc21eade6e4638066610f1626a910c6b6db878`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:19:57 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:19:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:19:59 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:21:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:21:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3530803da63720880f09e29040253e0f8fdebfb174978069f5b511d94216e`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02860751ea1196e0da1978bd80bdf7121b7e5769ff8713ca222c594035ff44`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fc1649eaa6b9174a6017d79b08ed23399aa70d3a40443f2b8843c1cdb65ba`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c032438917b21bcb582bd0cf1ef0ddcb31952a557601cd3cd347f4837c8dfa45`  
		Last Modified: Wed, 10 Aug 2022 15:26:47 GMT  
		Size: 134.4 MB (134407545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bac399186798527168b7633aec7516f048b4d5221c10e5fbbd41743fa767ff`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:1b56b2ccbb22387111844aa72865a1214560dcf6c6388c36279247d4b633eb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:1.6-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:a0818af2e0f8a13d4222356885970a613ec3b8610f0acafbda07ec20106981c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2451579016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e044ab27d86c37c4edaf9a01364962ee26df9b81fb003e4366acdb77f77413`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:18:30 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:18:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:18:32 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:19:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27460b61e7e0840b17c8d59299b4932215a5271d962024858263938f3140370b`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65d1a9c24024a1c33f1fd0e611f1b8dea64e66de1f9d448ef8b750f76c15bf`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006990ee1247492ce82d3a7c72562b9737e20b40d5b6c4c59264919bf3b48ed`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e610c6a735851c58863c1aa77010c7bfe7adeed65c34a96d12a60416f281d8`  
		Last Modified: Wed, 10 Aug 2022 15:26:09 GMT  
		Size: 134.7 MB (134683215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09da6580b4ce486d7a85b080bd0c32e5d645fdbfd95baa002c9a7de58ed2c93c`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7`

```console
$ docker pull julia@sha256:473c2adb82d0b9a9852f59aa6b16ef40e8b7f1b73aa61a611cc3369217e1fd6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.6.7` - linux; amd64

```console
$ docker pull julia@sha256:a33ccdfc660d2fbb36d7b811416e8c329a519935c685ea2b78e4649ee3fd6992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156447962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baf29e645cdf3ea1843317e4dd205abdd46a9517e333764f52efe46d1e4666`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:31 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 03:34:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c6af71d41cbf7d55043019d8a9c2af7620996a44311776c725591431fdcdad`  
		Last Modified: Tue, 23 Aug 2022 03:37:22 GMT  
		Size: 122.6 MB (122639906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; arm variant v7

```console
$ docker pull julia@sha256:23b46a7eed27310efd6ccc0b57e52e3094e7b084584194fb56dee6f553a233e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142488195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91f738fbe5e6176a15d2ce1eb6ec56393a9d47849c7838dc27d727268406033`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:00:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 18:00:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 18:00:52 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 18:01:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 18:01:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dd18e755cf320ec3c4a92559bb88648650871437863819346dff6c089befdd`  
		Last Modified: Tue, 23 Aug 2022 18:02:25 GMT  
		Size: 2.2 MB (2228774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f43c56ceb161c543292679ef861fe2bc6853a9f251d27cd5974ee6a0ebdaaa`  
		Last Modified: Tue, 23 Aug 2022 18:02:50 GMT  
		Size: 113.7 MB (113687689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:68ea505e8fc7975a8d22c4e4835f94ce4b19909642a2181f67a276c2e9e858db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148486570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc694b41b0dd18ed24140dd69bdd3340f0ecf746a24d626189e5f65eba5fdb6f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:32 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 04:28:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541cfdbd8d7dec8e159c1286d13d5d1abd6942c6b02cca72986ce5693d2f1d2`  
		Last Modified: Tue, 23 Aug 2022 04:31:26 GMT  
		Size: 116.2 MB (116213278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; 386

```console
$ docker pull julia@sha256:950b6532cf73ad077690e2088e27d1e9c15f2317a24ddbcc934ffca29385aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aefceeb9932d832416b48f44d01edacba83095c583ac6a220f6a96e34b05672`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:51 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 11:53:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:53:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879c19315299064e3c73e34f5ee1c2abfbb8ab802ecd12456385998dbc228765`  
		Last Modified: Tue, 23 Aug 2022 11:55:42 GMT  
		Size: 120.1 MB (120090724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:a0818af2e0f8a13d4222356885970a613ec3b8610f0acafbda07ec20106981c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2451579016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e044ab27d86c37c4edaf9a01364962ee26df9b81fb003e4366acdb77f77413`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:18:30 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:18:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:18:32 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:19:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27460b61e7e0840b17c8d59299b4932215a5271d962024858263938f3140370b`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65d1a9c24024a1c33f1fd0e611f1b8dea64e66de1f9d448ef8b750f76c15bf`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006990ee1247492ce82d3a7c72562b9737e20b40d5b6c4c59264919bf3b48ed`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e610c6a735851c58863c1aa77010c7bfe7adeed65c34a96d12a60416f281d8`  
		Last Modified: Wed, 10 Aug 2022 15:26:09 GMT  
		Size: 134.7 MB (134683215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09da6580b4ce486d7a85b080bd0c32e5d645fdbfd95baa002c9a7de58ed2c93c`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:a569e4731001467b267880dcc8d4f47289bd869a2001c38ce6a89c17a0fd271d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2812127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89843c1f4ebe099a51e15c435efc21eade6e4638066610f1626a910c6b6db878`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:19:57 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:19:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:19:59 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:21:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:21:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3530803da63720880f09e29040253e0f8fdebfb174978069f5b511d94216e`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02860751ea1196e0da1978bd80bdf7121b7e5769ff8713ca222c594035ff44`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fc1649eaa6b9174a6017d79b08ed23399aa70d3a40443f2b8843c1cdb65ba`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c032438917b21bcb582bd0cf1ef0ddcb31952a557601cd3cd347f4837c8dfa45`  
		Last Modified: Wed, 10 Aug 2022 15:26:47 GMT  
		Size: 134.4 MB (134407545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bac399186798527168b7633aec7516f048b4d5221c10e5fbbd41743fa767ff`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine`

```console
$ docker pull julia@sha256:abad5660f5a25b83328226f94c06f079ae52e1516c0964ca60425f8609470e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine` - linux; amd64

```console
$ docker pull julia@sha256:d3ce5d6d5d6f52656a02cf4c856bebd70b3bcbc03dcbe998dd8742fe6bc69a33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124634697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caf39300b6c77f62601cb1d00732814d855bb6adb601fcfaa30ee52fc91e391e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:44:03 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 09 Aug 2022 20:44:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:44:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f330082d37d521e85ed048135a49bb04735375b78ee4f62596d0fe91ddf609bd`  
		Last Modified: Tue, 09 Aug 2022 20:48:32 GMT  
		Size: 121.8 MB (121828643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine3.15`

```console
$ docker pull julia@sha256:3eaf1cf9731fbedfca9fc5ab8120a5f8168fd29ce23767061f64a02f6fb38091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:bbbffe7594e3fbb20aedd6c3ba81e9d5d327cd9f63728c7dbe809260d53d2ace
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124652106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b946aaf71e28d5eb07e343a7c2cee7b04d8ac744c4f1d362d64fd0e369931842`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:44:22 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 09 Aug 2022 20:44:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:44:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8ddc086b261016ce741f48368107159bdc66980c1f74a6324a65fc523cacb9`  
		Last Modified: Tue, 09 Aug 2022 20:49:06 GMT  
		Size: 121.8 MB (121828594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine3.16`

```console
$ docker pull julia@sha256:abad5660f5a25b83328226f94c06f079ae52e1516c0964ca60425f8609470e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:d3ce5d6d5d6f52656a02cf4c856bebd70b3bcbc03dcbe998dd8742fe6bc69a33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124634697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caf39300b6c77f62601cb1d00732814d855bb6adb601fcfaa30ee52fc91e391e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:44:03 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 09 Aug 2022 20:44:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:44:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f330082d37d521e85ed048135a49bb04735375b78ee4f62596d0fe91ddf609bd`  
		Last Modified: Tue, 09 Aug 2022 20:48:32 GMT  
		Size: 121.8 MB (121828643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-bullseye`

```console
$ docker pull julia@sha256:5d1506755eba77f8fde18de9fadaeaf12b259ab8a4782b0ef55569e30566fbf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.7-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:a33ccdfc660d2fbb36d7b811416e8c329a519935c685ea2b78e4649ee3fd6992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156447962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baf29e645cdf3ea1843317e4dd205abdd46a9517e333764f52efe46d1e4666`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:31 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 03:34:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c6af71d41cbf7d55043019d8a9c2af7620996a44311776c725591431fdcdad`  
		Last Modified: Tue, 23 Aug 2022 03:37:22 GMT  
		Size: 122.6 MB (122639906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:23b46a7eed27310efd6ccc0b57e52e3094e7b084584194fb56dee6f553a233e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142488195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91f738fbe5e6176a15d2ce1eb6ec56393a9d47849c7838dc27d727268406033`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:00:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 18:00:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 18:00:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 18:00:52 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 18:01:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 18:01:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dd18e755cf320ec3c4a92559bb88648650871437863819346dff6c089befdd`  
		Last Modified: Tue, 23 Aug 2022 18:02:25 GMT  
		Size: 2.2 MB (2228774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f43c56ceb161c543292679ef861fe2bc6853a9f251d27cd5974ee6a0ebdaaa`  
		Last Modified: Tue, 23 Aug 2022 18:02:50 GMT  
		Size: 113.7 MB (113687689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:68ea505e8fc7975a8d22c4e4835f94ce4b19909642a2181f67a276c2e9e858db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148486570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc694b41b0dd18ed24140dd69bdd3340f0ecf746a24d626189e5f65eba5fdb6f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:32 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 04:28:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541cfdbd8d7dec8e159c1286d13d5d1abd6942c6b02cca72986ce5693d2f1d2`  
		Last Modified: Tue, 23 Aug 2022 04:31:26 GMT  
		Size: 116.2 MB (116213278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; 386

```console
$ docker pull julia@sha256:950b6532cf73ad077690e2088e27d1e9c15f2317a24ddbcc934ffca29385aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aefceeb9932d832416b48f44d01edacba83095c583ac6a220f6a96e34b05672`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:51 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 11:53:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:53:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879c19315299064e3c73e34f5ee1c2abfbb8ab802ecd12456385998dbc228765`  
		Last Modified: Tue, 23 Aug 2022 11:55:42 GMT  
		Size: 120.1 MB (120090724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-buster`

```console
$ docker pull julia@sha256:ac755e4a7a7a8364d6826e97e7fc9c82f220f9edae2c856804bf7c98528f406f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.7-buster` - linux; amd64

```console
$ docker pull julia@sha256:ea3d52b8f06a09466df00b7de874240f263987e691873f96ecf7b5a911a45e4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154256163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101468a6f4cb99683b7f2788e6efc2df637727617bdd8e75f9d2ac60881a5973`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:34:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:50 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 03:35:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:35:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1964a73f39838efa7af98609a61ecf1ba3266086831790ee3de7c71c0e6ec711`  
		Last Modified: Tue, 23 Aug 2022 03:36:23 GMT  
		Size: 4.5 MB (4468185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e68eedbd2e9810c460134ace2381bf4c9bcdd7417bf6f922adaf1df3244a24`  
		Last Modified: Tue, 23 Aug 2022 03:37:51 GMT  
		Size: 122.6 MB (122649648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:29c5995ecdaffa347784776196e245c183c22da081deb197be84cb73aa08ef78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140253760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d1a8e51f38053ffdfc1a96e2fa653d06b75b0b6dc9c42e4f5c96a836043a0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 18:01:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 18:01:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 18:01:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 18:01:36 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 18:01:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 18:01:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6db4cf3a1e061a4bf1b4b5edf5b2aa7a5a9ad2239595b233a737fd58306baa`  
		Last Modified: Tue, 23 Aug 2022 18:03:04 GMT  
		Size: 3.8 MB (3811306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcdf7854ddd3e52b07c0a65ec22aeda15c7e65b7d9c58ab60ef805e3a7ba98`  
		Last Modified: Tue, 23 Aug 2022 18:03:28 GMT  
		Size: 113.7 MB (113695756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:d7ad07d964dce0935bc1daf7156f2a20c61d60c9cc468c41afc0dec3c3497cf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146481680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:001bb81f0eedd2e4e4d565e3579ef6ff4b961c48fca1e93c595cdfa758b38888`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:28:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:28:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:28:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:59 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 04:29:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:29:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee5ef9658b8af75e5d8cbd34d5a919e156f9da0588ac3a3b1501cd9b6a98081`  
		Last Modified: Tue, 23 Aug 2022 04:30:31 GMT  
		Size: 4.3 MB (4346922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b454e73f1e6abff01d763a6279aecc024eaf7c134f68ec9568c03509969c079`  
		Last Modified: Tue, 23 Aug 2022 04:31:54 GMT  
		Size: 116.2 MB (116222243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-buster` - linux; 386

```console
$ docker pull julia@sha256:91073a6d07f316382b34a9a5841958626881b6e296eba0555f57c617ca85a08f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.5 MB (152517064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df444009e83271e4ba28d60eba568e233882430e1a9987684e2f2d349850ac80`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:07 GMT
ADD file:69e3a870d6821a7b0d69402e3d7bc6488f1ed7d86dc5cf7f5f35d5868b72eaf3 in / 
# Tue, 23 Aug 2022 01:03:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:52:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:52:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:52:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:53:15 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 Aug 2022 11:53:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:53:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:46d42afa0260ad958104e1c87669868156eb23042a5c897146b1d7009ac682d9`  
		Last Modified: Tue, 23 Aug 2022 01:09:21 GMT  
		Size: 27.8 MB (27797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564ab79e374248c2778afffda8f2aa8a38a3c6e7d60c75426e41b9773387e20`  
		Last Modified: Tue, 23 Aug 2022 11:54:52 GMT  
		Size: 4.6 MB (4616209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbad84e0d169c9851168aa30b06b5c5eeb1fc007ef701390df4950677d592ecb`  
		Last Modified: Tue, 23 Aug 2022 11:56:10 GMT  
		Size: 120.1 MB (120103170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore`

```console
$ docker pull julia@sha256:8a4505711835e404073fd2c7295bd101f4ff396ef6afd77eb9b9d666b2dc16f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.6.7-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:a0818af2e0f8a13d4222356885970a613ec3b8610f0acafbda07ec20106981c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2451579016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e044ab27d86c37c4edaf9a01364962ee26df9b81fb003e4366acdb77f77413`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:18:30 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:18:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:18:32 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:19:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27460b61e7e0840b17c8d59299b4932215a5271d962024858263938f3140370b`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65d1a9c24024a1c33f1fd0e611f1b8dea64e66de1f9d448ef8b750f76c15bf`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006990ee1247492ce82d3a7c72562b9737e20b40d5b6c4c59264919bf3b48ed`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e610c6a735851c58863c1aa77010c7bfe7adeed65c34a96d12a60416f281d8`  
		Last Modified: Wed, 10 Aug 2022 15:26:09 GMT  
		Size: 134.7 MB (134683215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09da6580b4ce486d7a85b080bd0c32e5d645fdbfd95baa002c9a7de58ed2c93c`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:a569e4731001467b267880dcc8d4f47289bd869a2001c38ce6a89c17a0fd271d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2812127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89843c1f4ebe099a51e15c435efc21eade6e4638066610f1626a910c6b6db878`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:19:57 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:19:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:19:59 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:21:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:21:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3530803da63720880f09e29040253e0f8fdebfb174978069f5b511d94216e`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02860751ea1196e0da1978bd80bdf7121b7e5769ff8713ca222c594035ff44`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fc1649eaa6b9174a6017d79b08ed23399aa70d3a40443f2b8843c1cdb65ba`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c032438917b21bcb582bd0cf1ef0ddcb31952a557601cd3cd347f4837c8dfa45`  
		Last Modified: Wed, 10 Aug 2022 15:26:47 GMT  
		Size: 134.4 MB (134407545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bac399186798527168b7633aec7516f048b4d5221c10e5fbbd41743fa767ff`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore-1809`

```console
$ docker pull julia@sha256:a1f71101fad9124c34869394fb7ae1032fa4d5267a33752c9b76d61731a62c66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `julia:1.6.7-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:a569e4731001467b267880dcc8d4f47289bd869a2001c38ce6a89c17a0fd271d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2812127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89843c1f4ebe099a51e15c435efc21eade6e4638066610f1626a910c6b6db878`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:19:57 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:19:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:19:59 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:21:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:21:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3530803da63720880f09e29040253e0f8fdebfb174978069f5b511d94216e`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02860751ea1196e0da1978bd80bdf7121b7e5769ff8713ca222c594035ff44`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fc1649eaa6b9174a6017d79b08ed23399aa70d3a40443f2b8843c1cdb65ba`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c032438917b21bcb582bd0cf1ef0ddcb31952a557601cd3cd347f4837c8dfa45`  
		Last Modified: Wed, 10 Aug 2022 15:26:47 GMT  
		Size: 134.4 MB (134407545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bac399186798527168b7633aec7516f048b4d5221c10e5fbbd41743fa767ff`  
		Last Modified: Wed, 10 Aug 2022 15:26:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:1b56b2ccbb22387111844aa72865a1214560dcf6c6388c36279247d4b633eb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:1.6.7-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:a0818af2e0f8a13d4222356885970a613ec3b8610f0acafbda07ec20106981c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2451579016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e044ab27d86c37c4edaf9a01364962ee26df9b81fb003e4366acdb77f77413`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 15:18:30 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 Aug 2022 15:18:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 Aug 2022 15:18:32 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 Aug 2022 15:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:19:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27460b61e7e0840b17c8d59299b4932215a5271d962024858263938f3140370b`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65d1a9c24024a1c33f1fd0e611f1b8dea64e66de1f9d448ef8b750f76c15bf`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006990ee1247492ce82d3a7c72562b9737e20b40d5b6c4c59264919bf3b48ed`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e610c6a735851c58863c1aa77010c7bfe7adeed65c34a96d12a60416f281d8`  
		Last Modified: Wed, 10 Aug 2022 15:26:09 GMT  
		Size: 134.7 MB (134683215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09da6580b4ce486d7a85b080bd0c32e5d645fdbfd95baa002c9a7de58ed2c93c`  
		Last Modified: Wed, 10 Aug 2022 15:25:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8`

```console
$ docker pull julia@sha256:f063fdefb5a45ab75f3309c6e0a43f691a4100def0ae20caa233c74b26632bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.8` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-alpine`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.8-alpine` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-alpine3.15`

```console
$ docker pull julia@sha256:31b5056cbbd8f8af176d7ea40d7417ba6601e19c77858c8f0d3ced6a368e5002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.8-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:b7845cc320f6103c310ee765472bd55e09d7996a0844ccb932fbd85693faf26f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151954583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0757795c13b54d40903e67e7860639c8c4ed667060a620c7fa02ecbd0bfb610d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:50 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:30:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:30:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db51d58571ac8192edc30a955119ab6d5a7c2d8a2c8604f2a94708be1eeeaec`  
		Last Modified: Fri, 19 Aug 2022 00:33:17 GMT  
		Size: 149.1 MB (149131071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-alpine3.16`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.8-alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-bullseye`

```console
$ docker pull julia@sha256:43a3661152a3366a0be3694bf955d8b3cc8cfa765b7199bc90a4cbe46c2967fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.8-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-buster`

```console
$ docker pull julia@sha256:7caf803419e4a454079f5b009a3097af34be08e8b47585d5d1e3af576e4f4b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.8-buster` - linux; amd64

```console
$ docker pull julia@sha256:640642febd41f81d62607f5ce24fdca0e39b2060bcb3c56d49de52eb5603a903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179293925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef8073afa115ed02ab45dfa57b701ff85499d98010c3181a654267115db0ce2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:34:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1964a73f39838efa7af98609a61ecf1ba3266086831790ee3de7c71c0e6ec711`  
		Last Modified: Tue, 23 Aug 2022 03:36:23 GMT  
		Size: 4.5 MB (4468185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a104f3aff5ce20a6849b1477f4099735247ccfb1367958f9c488e5f40045fdd7`  
		Last Modified: Tue, 23 Aug 2022 03:36:45 GMT  
		Size: 147.7 MB (147687410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5eb5e78a2a9d028e17c0b5a07698e2337e532c7b4e7c5cbdcacef2769d7a9e05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171538865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3439f7910be37bb39acd736a62737601fc7c5730f34adc9e8a6967c12003bde9`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:28:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:28:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:28:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:10 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:28:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee5ef9658b8af75e5d8cbd34d5a919e156f9da0588ac3a3b1501cd9b6a98081`  
		Last Modified: Tue, 23 Aug 2022 04:30:31 GMT  
		Size: 4.3 MB (4346922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9958c3807c3314e6e599a4904ff947f31c08c358635ab79d9de63ab80f838b4f`  
		Last Modified: Tue, 23 Aug 2022 04:30:51 GMT  
		Size: 141.3 MB (141279428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8-buster` - linux; 386

```console
$ docker pull julia@sha256:d3ff6e52e422c4a0c78857deb1482f85c49ea045b6e4377555caa28e1548962e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176958712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94b068ddad4812a4c890228329edecdcd8be47afd6066284340d46d33d5ee5`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:07 GMT
ADD file:69e3a870d6821a7b0d69402e3d7bc6488f1ed7d86dc5cf7f5f35d5868b72eaf3 in / 
# Tue, 23 Aug 2022 01:03:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:52:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:52:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:52:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:25 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:46d42afa0260ad958104e1c87669868156eb23042a5c897146b1d7009ac682d9`  
		Last Modified: Tue, 23 Aug 2022 01:09:21 GMT  
		Size: 27.8 MB (27797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564ab79e374248c2778afffda8f2aa8a38a3c6e7d60c75426e41b9773387e20`  
		Last Modified: Tue, 23 Aug 2022 11:54:52 GMT  
		Size: 4.6 MB (4616209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c3b90157dbe01d07e902812add81f9d5607811adfd3e387d19bad31225a3c0`  
		Last Modified: Tue, 23 Aug 2022 11:55:10 GMT  
		Size: 144.5 MB (144544818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-windowsservercore`

```console
$ docker pull julia@sha256:aeaeacee9115fb97e300dadcba1ce584f70785a9010cfbf2ba6ab8d2b67a23d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.8-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-windowsservercore-1809`

```console
$ docker pull julia@sha256:bb2ec07816d9c5d0bd9f326119a53882a494cb038e2a6cdcd4a832720fd002b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `julia:1.8-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:d456bc1037ec50a9558c1143a8dfb6712820851fae28aa4773ce45ddeb8d40e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:1.8-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0`

```console
$ docker pull julia@sha256:f063fdefb5a45ab75f3309c6e0a43f691a4100def0ae20caa233c74b26632bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.8.0` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-alpine`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.8.0-alpine` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-alpine3.15`

```console
$ docker pull julia@sha256:31b5056cbbd8f8af176d7ea40d7417ba6601e19c77858c8f0d3ced6a368e5002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.8.0-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:b7845cc320f6103c310ee765472bd55e09d7996a0844ccb932fbd85693faf26f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151954583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0757795c13b54d40903e67e7860639c8c4ed667060a620c7fa02ecbd0bfb610d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:50 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:30:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:30:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db51d58571ac8192edc30a955119ab6d5a7c2d8a2c8604f2a94708be1eeeaec`  
		Last Modified: Fri, 19 Aug 2022 00:33:17 GMT  
		Size: 149.1 MB (149131071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-alpine3.16`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.8.0-alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-bullseye`

```console
$ docker pull julia@sha256:43a3661152a3366a0be3694bf955d8b3cc8cfa765b7199bc90a4cbe46c2967fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.8.0-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-buster`

```console
$ docker pull julia@sha256:7caf803419e4a454079f5b009a3097af34be08e8b47585d5d1e3af576e4f4b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.8.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:640642febd41f81d62607f5ce24fdca0e39b2060bcb3c56d49de52eb5603a903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179293925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef8073afa115ed02ab45dfa57b701ff85499d98010c3181a654267115db0ce2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:34:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1964a73f39838efa7af98609a61ecf1ba3266086831790ee3de7c71c0e6ec711`  
		Last Modified: Tue, 23 Aug 2022 03:36:23 GMT  
		Size: 4.5 MB (4468185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a104f3aff5ce20a6849b1477f4099735247ccfb1367958f9c488e5f40045fdd7`  
		Last Modified: Tue, 23 Aug 2022 03:36:45 GMT  
		Size: 147.7 MB (147687410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5eb5e78a2a9d028e17c0b5a07698e2337e532c7b4e7c5cbdcacef2769d7a9e05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171538865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3439f7910be37bb39acd736a62737601fc7c5730f34adc9e8a6967c12003bde9`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:28:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:28:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:28:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:10 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:28:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee5ef9658b8af75e5d8cbd34d5a919e156f9da0588ac3a3b1501cd9b6a98081`  
		Last Modified: Tue, 23 Aug 2022 04:30:31 GMT  
		Size: 4.3 MB (4346922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9958c3807c3314e6e599a4904ff947f31c08c358635ab79d9de63ab80f838b4f`  
		Last Modified: Tue, 23 Aug 2022 04:30:51 GMT  
		Size: 141.3 MB (141279428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0-buster` - linux; 386

```console
$ docker pull julia@sha256:d3ff6e52e422c4a0c78857deb1482f85c49ea045b6e4377555caa28e1548962e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176958712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94b068ddad4812a4c890228329edecdcd8be47afd6066284340d46d33d5ee5`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:07 GMT
ADD file:69e3a870d6821a7b0d69402e3d7bc6488f1ed7d86dc5cf7f5f35d5868b72eaf3 in / 
# Tue, 23 Aug 2022 01:03:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:52:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:52:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:52:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:25 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:46d42afa0260ad958104e1c87669868156eb23042a5c897146b1d7009ac682d9`  
		Last Modified: Tue, 23 Aug 2022 01:09:21 GMT  
		Size: 27.8 MB (27797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564ab79e374248c2778afffda8f2aa8a38a3c6e7d60c75426e41b9773387e20`  
		Last Modified: Tue, 23 Aug 2022 11:54:52 GMT  
		Size: 4.6 MB (4616209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c3b90157dbe01d07e902812add81f9d5607811adfd3e387d19bad31225a3c0`  
		Last Modified: Tue, 23 Aug 2022 11:55:10 GMT  
		Size: 144.5 MB (144544818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-windowsservercore`

```console
$ docker pull julia@sha256:aeaeacee9115fb97e300dadcba1ce584f70785a9010cfbf2ba6ab8d2b67a23d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:1.8.0-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.8.0-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:bb2ec07816d9c5d0bd9f326119a53882a494cb038e2a6cdcd4a832720fd002b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `julia:1.8.0-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.8.0-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:d456bc1037ec50a9558c1143a8dfb6712820851fae28aa4773ce45ddeb8d40e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:1.8.0-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.15`

```console
$ docker pull julia@sha256:31b5056cbbd8f8af176d7ea40d7417ba6601e19c77858c8f0d3ced6a368e5002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:b7845cc320f6103c310ee765472bd55e09d7996a0844ccb932fbd85693faf26f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151954583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0757795c13b54d40903e67e7860639c8c4ed667060a620c7fa02ecbd0bfb610d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:50 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:30:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:30:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db51d58571ac8192edc30a955119ab6d5a7c2d8a2c8604f2a94708be1eeeaec`  
		Last Modified: Fri, 19 Aug 2022 00:33:17 GMT  
		Size: 149.1 MB (149131071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.16`

```console
$ docker pull julia@sha256:ae97cf89b550b3f7adab69ae29cd145bd734e0a3e4f6039c80839febffe1abe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:3f4f3d8450bc609e40c556779cc3c577c2306af9ef7c262dacc7f43fd0310bb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151937102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba0a4c493779971024c7e45ad71d80dbbb1383e45953425676b42c56f0444d7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 19 Aug 2022 00:29:26 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:29:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-musl-x86_64.tar.gz'; 			sha256='d60de3a1c522e30655babdda2d80cf756848983ea57ff38eca8e60108f5001b6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 19 Aug 2022 00:29:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a13f32f792eae2fbd538bd655db1d95b6abfc217cded086228e8b73b67a42b6`  
		Last Modified: Fri, 19 Aug 2022 00:32:28 GMT  
		Size: 149.1 MB (149131048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:bullseye`

```console
$ docker pull julia@sha256:43a3661152a3366a0be3694bf955d8b3cc8cfa765b7199bc90a4cbe46c2967fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:bullseye` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:7caf803419e4a454079f5b009a3097af34be08e8b47585d5d1e3af576e4f4b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:640642febd41f81d62607f5ce24fdca0e39b2060bcb3c56d49de52eb5603a903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179293925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef8073afa115ed02ab45dfa57b701ff85499d98010c3181a654267115db0ce2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:34:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:34:04 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:34:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1964a73f39838efa7af98609a61ecf1ba3266086831790ee3de7c71c0e6ec711`  
		Last Modified: Tue, 23 Aug 2022 03:36:23 GMT  
		Size: 4.5 MB (4468185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a104f3aff5ce20a6849b1477f4099735247ccfb1367958f9c488e5f40045fdd7`  
		Last Modified: Tue, 23 Aug 2022 03:36:45 GMT  
		Size: 147.7 MB (147687410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5eb5e78a2a9d028e17c0b5a07698e2337e532c7b4e7c5cbdcacef2769d7a9e05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171538865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3439f7910be37bb39acd736a62737601fc7c5730f34adc9e8a6967c12003bde9`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:28:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:28:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:28:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:28:10 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:28:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:28:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee5ef9658b8af75e5d8cbd34d5a919e156f9da0588ac3a3b1501cd9b6a98081`  
		Last Modified: Tue, 23 Aug 2022 04:30:31 GMT  
		Size: 4.3 MB (4346922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9958c3807c3314e6e599a4904ff947f31c08c358635ab79d9de63ab80f838b4f`  
		Last Modified: Tue, 23 Aug 2022 04:30:51 GMT  
		Size: 141.3 MB (141279428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:d3ff6e52e422c4a0c78857deb1482f85c49ea045b6e4377555caa28e1548962e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.0 MB (176958712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94b068ddad4812a4c890228329edecdcd8be47afd6066284340d46d33d5ee5`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:07 GMT
ADD file:69e3a870d6821a7b0d69402e3d7bc6488f1ed7d86dc5cf7f5f35d5868b72eaf3 in / 
# Tue, 23 Aug 2022 01:03:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:52:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:52:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:52:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:52:25 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:46d42afa0260ad958104e1c87669868156eb23042a5c897146b1d7009ac682d9`  
		Last Modified: Tue, 23 Aug 2022 01:09:21 GMT  
		Size: 27.8 MB (27797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564ab79e374248c2778afffda8f2aa8a38a3c6e7d60c75426e41b9773387e20`  
		Last Modified: Tue, 23 Aug 2022 11:54:52 GMT  
		Size: 4.6 MB (4616209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c3b90157dbe01d07e902812add81f9d5607811adfd3e387d19bad31225a3c0`  
		Last Modified: Tue, 23 Aug 2022 11:55:10 GMT  
		Size: 144.5 MB (144544818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:f063fdefb5a45ab75f3309c6e0a43f691a4100def0ae20caa233c74b26632bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:8caf32e8eda8a6b80a63c4290007b92330fd793f351c05889c01113bb20734f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181485134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ef895b2930c675dffe89c4173d5b6bf743d7973e52875623d3677ce045641c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:33:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 03:33:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 03:33:35 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 03:33:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 03:33:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4feaea1a05bbbe172701dfdffbd2ec7c15f8c4b76a7d0a705d32233318609`  
		Last Modified: Tue, 23 Aug 2022 03:35:46 GMT  
		Size: 2.4 MB (2426571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c302e857337d494b6c2598f6ac02142a28f2b52175951072fba6e75e382c751`  
		Last Modified: Tue, 23 Aug 2022 03:36:08 GMT  
		Size: 147.7 MB (147677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:67a206be774c0e3b5210027ab147edea3ad2339cc19cd5bb04d11081f9886e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.5 MB (173542376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b2546d7bc677c82c2869543804f74578a06ff9bb0685369cb63050f48037f7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:27:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 04:27:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:27:30 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 04:27:31 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 04:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 04:27:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e0f19ade481c09578999bd5144195ece422b1ee18453296d410fbd989d807`  
		Last Modified: Tue, 23 Aug 2022 04:29:52 GMT  
		Size: 2.2 MB (2209504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413a6c21b03caf4e86edc49d480949ca2639e751a76476de28c8d65368cd428`  
		Last Modified: Tue, 23 Aug 2022 04:30:13 GMT  
		Size: 141.3 MB (141269084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:ac97c7338d08bb7c7de023a116c9ac45436ca3dd6a3bf5b783a3f178ed7f9245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179255595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b44d452e0dd3e418bd7871c005a6824c2ceab244618295486b5450ece6014ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:51:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 Aug 2022 11:51:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:51:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 Aug 2022 11:51:45 GMT
ENV JULIA_VERSION=1.8.0
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-linux-x86_64.tar.gz'; 			sha256='e80d732ccb7f79e000d798cb8b656dc3641ab59516d6e4e52e16765017892a00'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-linux-aarch64.tar.gz'; 			sha256='e003cfb8680af1a65c3be55b53a48cc5186300adaaba8926209800b4d1f4ca7a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-linux-i686.tar.gz'; 			sha256='68866069969aec0c249fedc23eecceaa818a83cc92650d3561d4d47d8a586301'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 Aug 2022 11:52:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd13a7a7280a8ce197176210f79f79dc7d24ee938e4e04785d6e2fb6c7e04c33`  
		Last Modified: Tue, 23 Aug 2022 11:54:15 GMT  
		Size: 2.3 MB (2326542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df4eb4948fc6f863dcd99a6127bb7b473abc61462a31f1b7cce6ddd9abca54`  
		Last Modified: Tue, 23 Aug 2022 11:54:34 GMT  
		Size: 144.5 MB (144541736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore`

```console
$ docker pull julia@sha256:aeaeacee9115fb97e300dadcba1ce584f70785a9010cfbf2ba6ab8d2b67a23d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `julia:windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:bb2ec07816d9c5d0bd9f326119a53882a494cb038e2a6cdcd4a832720fd002b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull julia@sha256:48d0550719b4eaa16edb377655fc4df914f68c03d3ea64ae02c9ddce215b8592
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2837955846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c5e511f6ac246c153031243e2b7a93744b56b1794afc4de25b95a540092e20`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:17:43 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:17:44 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:20:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:20:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6346496c22f2588130d379f898561733b3bbc4c992abeeed815814a2b5d93e`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a530de1ed793d0d45644bcc65981578559949a5b58be5e206c942d1887348ac8`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57df4b1347f7eee5b858c1f8614965f8dc41601eb2807feeb0eca97e51b2b66`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f471d4c28c8a9c03348ad64babbdfb9917f8f3e6983d943ee8f8b79e9a3151d1`  
		Last Modified: Fri, 19 Aug 2022 00:22:28 GMT  
		Size: 160.2 MB (160236071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db02e18520da67cbf7836ae4b5a70246d418a8b661c8f17c69dd429148882f6`  
		Last Modified: Fri, 19 Aug 2022 00:21:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:d456bc1037ec50a9558c1143a8dfb6712820851fae28aa4773ce45ddeb8d40e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:f6241fcf25f0f14ee094adf4a0872efe74ef72d34fa74d55849640d6903ab3ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477394509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005dec4146ebaaffc984e7f1a3d00f1ab3e1126d87a14ddbe8c53d33a5e9df3d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 19 Aug 2022 00:16:00 GMT
ENV JULIA_VERSION=1.8.0
# Fri, 19 Aug 2022 00:16:01 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-win64.exe
# Fri, 19 Aug 2022 00:16:03 GMT
ENV JULIA_SHA256=a1699278e4884578c10580cf19f8d42401abce78f459c416998221902ea26d38
# Fri, 19 Aug 2022 00:17:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 19 Aug 2022 00:17:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06f2d471be84413e3e4e6902f7bd63ab118d4c43d14367861367ede14cbff58`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c99f603d86e2c9fe398b1e62de63ea5c4b37fa1bc0a74c9dd03af68cf773`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daa8117b050cc6db64f65f4d4afa44e0c1487d694fae17d8eabcf2afcf44610`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60d4abe59ff41e01dbdc4fee230b6ca75ff4b3481d4d294c7c8a722d0e45092`  
		Last Modified: Fri, 19 Aug 2022 00:21:39 GMT  
		Size: 160.5 MB (160498317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1fb16fac4eec8b752d2a6a6ff9c4b8394d9404339102879b3165ebd22f9667`  
		Last Modified: Fri, 19 Aug 2022 00:21:04 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
