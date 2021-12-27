<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.14`](#julia1-alpine314)
-	[`julia:1-alpine3.15`](#julia1-alpine315)
-	[`julia:1-bullseye`](#julia1-bullseye)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-windowsservercore`](#julia1-windowsservercore)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2016`](#julia1-windowsservercore-ltsc2016)
-	[`julia:1-windowsservercore-ltsc2022`](#julia1-windowsservercore-ltsc2022)
-	[`julia:1.6`](#julia16)
-	[`julia:1.6-alpine`](#julia16-alpine)
-	[`julia:1.6-alpine3.14`](#julia16-alpine314)
-	[`julia:1.6-alpine3.15`](#julia16-alpine315)
-	[`julia:1.6-bullseye`](#julia16-bullseye)
-	[`julia:1.6-buster`](#julia16-buster)
-	[`julia:1.6-windowsservercore`](#julia16-windowsservercore)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2016`](#julia16-windowsservercore-ltsc2016)
-	[`julia:1.6-windowsservercore-ltsc2022`](#julia16-windowsservercore-ltsc2022)
-	[`julia:1.6.5`](#julia165)
-	[`julia:1.6.5-alpine`](#julia165-alpine)
-	[`julia:1.6.5-alpine3.14`](#julia165-alpine314)
-	[`julia:1.6.5-alpine3.15`](#julia165-alpine315)
-	[`julia:1.6.5-bullseye`](#julia165-bullseye)
-	[`julia:1.6.5-buster`](#julia165-buster)
-	[`julia:1.6.5-windowsservercore`](#julia165-windowsservercore)
-	[`julia:1.6.5-windowsservercore-1809`](#julia165-windowsservercore-1809)
-	[`julia:1.6.5-windowsservercore-ltsc2016`](#julia165-windowsservercore-ltsc2016)
-	[`julia:1.6.5-windowsservercore-ltsc2022`](#julia165-windowsservercore-ltsc2022)
-	[`julia:1.7`](#julia17)
-	[`julia:1.7-alpine`](#julia17-alpine)
-	[`julia:1.7-alpine3.14`](#julia17-alpine314)
-	[`julia:1.7-alpine3.15`](#julia17-alpine315)
-	[`julia:1.7-bullseye`](#julia17-bullseye)
-	[`julia:1.7-buster`](#julia17-buster)
-	[`julia:1.7-windowsservercore`](#julia17-windowsservercore)
-	[`julia:1.7-windowsservercore-1809`](#julia17-windowsservercore-1809)
-	[`julia:1.7-windowsservercore-ltsc2016`](#julia17-windowsservercore-ltsc2016)
-	[`julia:1.7-windowsservercore-ltsc2022`](#julia17-windowsservercore-ltsc2022)
-	[`julia:1.7.1`](#julia171)
-	[`julia:1.7.1-alpine`](#julia171-alpine)
-	[`julia:1.7.1-alpine3.14`](#julia171-alpine314)
-	[`julia:1.7.1-alpine3.15`](#julia171-alpine315)
-	[`julia:1.7.1-bullseye`](#julia171-bullseye)
-	[`julia:1.7.1-buster`](#julia171-buster)
-	[`julia:1.7.1-windowsservercore`](#julia171-windowsservercore)
-	[`julia:1.7.1-windowsservercore-1809`](#julia171-windowsservercore-1809)
-	[`julia:1.7.1-windowsservercore-ltsc2016`](#julia171-windowsservercore-ltsc2016)
-	[`julia:1.7.1-windowsservercore-ltsc2022`](#julia171-windowsservercore-ltsc2022)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.14`](#juliaalpine314)
-	[`julia:alpine3.15`](#juliaalpine315)
-	[`julia:bullseye`](#juliabullseye)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore`](#juliawindowsservercore)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)
-	[`julia:windowsservercore-ltsc2022`](#juliawindowsservercore-ltsc2022)

## `julia:1`

```console
$ docker pull julia@sha256:545895061073bc6adbae53c0cbe2cac62aa8afd3f204ff745e31d0699969f349
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.14`

```console
$ docker pull julia@sha256:8d694f350ed9d13a457d7d33a951594ef7b55cd8a60b5dac116366ffe2fc6920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:4328442d3c3eb9de31aec772546436b7a9b38ba319a274ad8282e7388c7747c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134595199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5683a72eb9212724b391b9bbe160fecbec5b864b8f7b4432d2d5cf73e75359`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1053bc232f4e5495d158a20c62c5fca1d2b6f2741a93580531bf266910062a8f`  
		Last Modified: Mon, 27 Dec 2021 18:48:49 GMT  
		Size: 131.8 MB (131772218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.15`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-bullseye`

```console
$ docker pull julia@sha256:6bab698fdb707d9988eddac51ec36ec7261e8b2c46510c3769cadd9cc3708729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:f0a5766c86b1223bdd91767baa3f3e7c7b914fed37990f9f559ac207d3d88937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:8cfa444dfe1e3362b079fbec07fcc7fc47f6061d80425a2c89001e949299bd03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164156514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc405e9ce723306cf702dd4a1a7f29e9caa82c7eb9e908d93382b6c8a9a15733`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:35 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:45:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d90b7a76b8623c863a0af16dcdde2098d7b6156e63ae932bae0682bf40db9`  
		Last Modified: Tue, 21 Dec 2021 02:34:37 GMT  
		Size: 4.5 MB (4458501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a8d66b0aad5d66842ae0e66b6ce78557fee5e7fbc807d1fdb678afe670792`  
		Last Modified: Mon, 27 Dec 2021 18:47:32 GMT  
		Size: 132.5 MB (132544290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:7a4ef7c24e16a63d9a6b8fce489b5359d7ac31e6be2e1fdc78b7f21321714bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155918945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d323828aa7b36c87d276d0dd64eebb7353d57c1965bc6fb36c91793b5bccbe74`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:52:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:52:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:52:32 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:40:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59091731f7a5e363cc0dd5a19d3e56f18bc4165c020fa2c62a2c23a6a8d55a`  
		Last Modified: Tue, 21 Dec 2021 10:55:14 GMT  
		Size: 4.3 MB (4338189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c8ac4ad3e6cbeda7573be619cb77e0c983ee2038d4ed72440cb59f763cec4e`  
		Last Modified: Mon, 27 Dec 2021 17:42:34 GMT  
		Size: 125.7 MB (125657607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:d96339edf04f747dbb364f9c34c616341d65ea9aefa14a7936f1c8ef7fd59fbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161209682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9195370cc3121df2b7f9aac958404af4c50c8c904cc72ab039807c49280eac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:45:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:45:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:45:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:17 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a2d4803cd1b772d17b3feabe820fe1067f750917bf28c21c5d5f468afa7fe8`  
		Last Modified: Tue, 21 Dec 2021 07:49:07 GMT  
		Size: 4.6 MB (4611023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad77c239750f92c468b5b65093a40d17fec6cb412e71a13ec5d250b728bf666`  
		Last Modified: Mon, 27 Dec 2021 17:41:45 GMT  
		Size: 128.8 MB (128794086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore`

```console
$ docker pull julia@sha256:cade52ef6d84e8447cc04650915a7076ee9bdb9b945bcae2a2ed6d559664742a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:0ec7efc01d8fe5085ffeca6137c838136653f2ccabb9e559673f6c434d5fdb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:1fefcc3c73f90296644ee58bcb1046c76116e0f5604ba82b78c8c8e3c2b648ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:f02889aee8ceaab805f4b9379afe9a4f15e3ef86313a305cd66c143b1b13626c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `julia:1-windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:60aeb8e45be9ef39f4d9d67c5bb5f8796dcfa11b5b7fc4d2b5aa7c5494e13ded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:2ef5a0f19f81703f04094c78657b8443e963f7c3b44d6007d0945c7f70bc028a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155401867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5532da26a08b117a16c29c151bb8e13ae160b17f4144bd05707cbf83325e7274`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:58:16 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:58:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 21:58:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38142823e55e64a3bc27c80730299eb1da2984e83f9406ed33ed120d632da445`  
		Last Modified: Wed, 22 Dec 2021 22:00:58 GMT  
		Size: 121.6 MB (121618783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:8311ae235193bfc27bd09087929a37453b4247bf4fa3b56df25c82599e36f08c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141549810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8819044f958a8d0a7bd4db01f03929fb0cd51595a37a0799ccb75aa23ae2249`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:25:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:25:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:25:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:25:43 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Dec 2021 05:58:01 GMT
ENV JULIA_VERSION=1.6.5
# Thu, 23 Dec 2021 05:58:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Dec 2021 05:58:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f37016379049dbd4608d5a4cf9d671487875c1e04a4982557d166d0c5fe138`  
		Last Modified: Tue, 21 Dec 2021 07:28:31 GMT  
		Size: 2.2 MB (2227504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e133e7f3cba6914373c6e9a46ce04ba26872c19a26e94a2e7a1fefd7f17b14`  
		Last Modified: Thu, 23 Dec 2021 06:01:37 GMT  
		Size: 112.8 MB (112761491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a471ad9988b9d589a4ecfc327a6720e6ff716ddfac7cf0b4bd5932eee78d8e9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147627114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c8dea12468b3b39ca9e446a6dcf830516f2a25039d67d670b44b2b423316e2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 19:28:36 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:28:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 19:28:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b6453ae077e7d1f5085e555eccc55c5feeef605098ecb98bbe91c91759d15`  
		Last Modified: Wed, 22 Dec 2021 19:30:22 GMT  
		Size: 115.2 MB (115170876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:ebac08a52e3ba80badffbf207840e27bb1aeba099c25cef49c4c6b488a38e22c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154155382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2f7461565250c49d111ff71d68cdcf7b979d13f410290d287ba7c7b64e5d0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 20:47:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 20:47:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 20:47:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe4f2dda07f20e17a43e7bc704e79462ec5bfc58b4c585d4280450b36ae6d2`  
		Last Modified: Wed, 22 Dec 2021 20:49:50 GMT  
		Size: 119.3 MB (119255036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:7eea907b57a8580108e6828c9cf2211d605e40560cca8bee98b8debddd81348c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325192216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c112159bff771c5eaaa4dc6c6081da65c73b3eaf80d7791d77dab86ef73614c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:16:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:16:10 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:16:12 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:17:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5bc799d7a6b72fe2a92e227ce3e72eda15852cca648edbffde4f5196b8fd28`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d3a60fc4823edb2dc48e7dc79f2084d47d721aaa552207214459580e2fdd0`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a911a2357de34787001fdca732d87189a8bf1f460da7dab9cdec04b15f583e3b`  
		Last Modified: Wed, 22 Dec 2021 19:24:32 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c27eac142ebf7fc318fb2b32c37051be9434d7f9df6d33107d57c33d670d3`  
		Last Modified: Wed, 22 Dec 2021 19:26:59 GMT  
		Size: 134.4 MB (134413551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07a0883745cb931a41259b2fe70194ae1270f6ed3ab915d79e4ba168a63933e`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:ebfaf0856b165128d116e72cf34bfc013b26d00605d354c951d67f52e93a00dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842770402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a3633b42ac1bb94c430d603bb2248359af77459a0f94be51da03a0e2cdf359`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:18:07 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:18:08 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:18:10 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:20:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec01c86598057b0ba8a30af6624599148001c73b4397623970c17a9b6822c3c`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de51ecc8ca2d4ec960fecf7e7013f4032107c3aa5050d40d8eff7f5d16a831ab`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182ac5c826097666bd787f2234ab9423fb2d2ea72d697ae62d95319efbba475`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4143a01766a217c2a0da621057725e5a229f51c1c8778523f3eea0b04060d`  
		Last Modified: Wed, 22 Dec 2021 19:27:39 GMT  
		Size: 134.2 MB (134158790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a9a3732552b71e088371a52624c70cf32d1d7ed1596cee002b0b248b1cf6d`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:ebf47edb8b2258a6ff50fbf922a30ebf9c40b73fdc18db37c619a1f7c002af62
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408845728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57f595200ff30dcd7b6c90428bcd4aabbe8fb549c3576a48786067f34345172`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:21:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:21:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:21:07 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebef7e05ef5388d95b79785f0dd1f495fa64a0513bf7f2b6eb7b81cc438f93f2`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b69a5c57d23ff9757738234b8d6a6a356a6a07f5e0e2f0c4c62e785b6b54`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb413f4ff9442af4fb91c7ccd16c0aa2e30f45fcc8e56e6c8fd02798416be37`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539c8cb1c574e3ab73950b0c7d634d3dc27dba154c1bcd572ccaed386fa642`  
		Last Modified: Wed, 22 Dec 2021 19:30:18 GMT  
		Size: 134.1 MB (134123877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc8f9569ec24361b165bc28ffb36986ba71988f9f962207c555e6c6c57a714`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine`

```console
$ docker pull julia@sha256:9caa4089b61c4ee893ab898cb4c0470d716f714e8a6e616483458770339f81cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine` - linux; amd64

```console
$ docker pull julia@sha256:a5b375a5c874d93c0444dbdca526d474a8dc3bd87a00a694273d349bb01c93c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123688600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2c761d44dc029f3d9445e6d6b0c786a67e2bea4d9cfebe39a3847e469099ef`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:59:14 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.5-musl-x86_64.tar.gz'; 			sha256='e38eece6f9f20c7472caf3f8f74a99ad0880921c28e1301461fa7af919880383'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 22 Dec 2021 21:59:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6203055cf397dc97a4889e9a4f7287312c95034ff8f4399131d85e5c14377a1`  
		Last Modified: Wed, 22 Dec 2021 22:01:55 GMT  
		Size: 120.9 MB (120870187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.14`

```console
$ docker pull julia@sha256:21f3298f06efc4345863d3794a8473a9afd6bef31fa3c1c1d80230d6c6a98670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:6a8946aeffb6ea6b7ff18a6e0d039eb1da08415c6496256c782ca58f7f267d93
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123693368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fecc22608b4515475f74e89cd9201c5abf9c0eda7629c3e2c8f7a4fd1026eb8`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:59:37 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.5-musl-x86_64.tar.gz'; 			sha256='e38eece6f9f20c7472caf3f8f74a99ad0880921c28e1301461fa7af919880383'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 22 Dec 2021 21:59:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4463ae12c2ce8489f970877c2f5b1194a28ec4234be9e0ac4adc9bda3500a8`  
		Last Modified: Wed, 22 Dec 2021 22:02:29 GMT  
		Size: 120.9 MB (120870387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.15`

```console
$ docker pull julia@sha256:9caa4089b61c4ee893ab898cb4c0470d716f714e8a6e616483458770339f81cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:a5b375a5c874d93c0444dbdca526d474a8dc3bd87a00a694273d349bb01c93c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123688600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2c761d44dc029f3d9445e6d6b0c786a67e2bea4d9cfebe39a3847e469099ef`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:59:14 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.5-musl-x86_64.tar.gz'; 			sha256='e38eece6f9f20c7472caf3f8f74a99ad0880921c28e1301461fa7af919880383'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 22 Dec 2021 21:59:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6203055cf397dc97a4889e9a4f7287312c95034ff8f4399131d85e5c14377a1`  
		Last Modified: Wed, 22 Dec 2021 22:01:55 GMT  
		Size: 120.9 MB (120870187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-bullseye`

```console
$ docker pull julia@sha256:e2db61d5e0de29272be9bbc6d176eed0e17cb61920b70b8632bcbe458ede283b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:2ef5a0f19f81703f04094c78657b8443e963f7c3b44d6007d0945c7f70bc028a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155401867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5532da26a08b117a16c29c151bb8e13ae160b17f4144bd05707cbf83325e7274`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:58:16 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:58:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 21:58:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38142823e55e64a3bc27c80730299eb1da2984e83f9406ed33ed120d632da445`  
		Last Modified: Wed, 22 Dec 2021 22:00:58 GMT  
		Size: 121.6 MB (121618783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:8311ae235193bfc27bd09087929a37453b4247bf4fa3b56df25c82599e36f08c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141549810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8819044f958a8d0a7bd4db01f03929fb0cd51595a37a0799ccb75aa23ae2249`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:25:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:25:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:25:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:25:43 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Dec 2021 05:58:01 GMT
ENV JULIA_VERSION=1.6.5
# Thu, 23 Dec 2021 05:58:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Dec 2021 05:58:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f37016379049dbd4608d5a4cf9d671487875c1e04a4982557d166d0c5fe138`  
		Last Modified: Tue, 21 Dec 2021 07:28:31 GMT  
		Size: 2.2 MB (2227504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e133e7f3cba6914373c6e9a46ce04ba26872c19a26e94a2e7a1fefd7f17b14`  
		Last Modified: Thu, 23 Dec 2021 06:01:37 GMT  
		Size: 112.8 MB (112761491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a471ad9988b9d589a4ecfc327a6720e6ff716ddfac7cf0b4bd5932eee78d8e9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147627114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c8dea12468b3b39ca9e446a6dcf830516f2a25039d67d670b44b2b423316e2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 19:28:36 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:28:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 19:28:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b6453ae077e7d1f5085e555eccc55c5feeef605098ecb98bbe91c91759d15`  
		Last Modified: Wed, 22 Dec 2021 19:30:22 GMT  
		Size: 115.2 MB (115170876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ebac08a52e3ba80badffbf207840e27bb1aeba099c25cef49c4c6b488a38e22c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154155382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2f7461565250c49d111ff71d68cdcf7b979d13f410290d287ba7c7b64e5d0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 20:47:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 20:47:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 20:47:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe4f2dda07f20e17a43e7bc704e79462ec5bfc58b4c585d4280450b36ae6d2`  
		Last Modified: Wed, 22 Dec 2021 20:49:50 GMT  
		Size: 119.3 MB (119255036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:ec3c667a63853ae0be71ee4ba759e0cce1ecc5f0382859b70473e39ceb4c48dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:f860e513a73b32a469bbf3e60c41934c9fbf90ae98d458261a5f78925a6794d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153237394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d9c86a8289f9a2582a82c8e869c2433dd85c9597447f5957c92f274f9d5279`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:58:50 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 21:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d90b7a76b8623c863a0af16dcdde2098d7b6156e63ae932bae0682bf40db9`  
		Last Modified: Tue, 21 Dec 2021 02:34:37 GMT  
		Size: 4.5 MB (4458501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9a921cde994753f96149f95af939deddcce1eec091151ab4ac295859387671`  
		Last Modified: Wed, 22 Dec 2021 22:01:27 GMT  
		Size: 121.6 MB (121625170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a670efe718cc2152fabacf224bf30ea847c63e6bc1b91d6f76a0408bb3f262c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139323412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b228efb7d262f0b4529e2d9130a2ae5e77b78a108a2c8e5d235087ed77ab7901`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:27:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:27:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:27:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:27:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Dec 2021 05:59:02 GMT
ENV JULIA_VERSION=1.6.5
# Thu, 23 Dec 2021 05:59:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Dec 2021 05:59:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb00b7b6f8221655a7461d12bc7c3eb31d355271d28a924892c78d693001876f`  
		Last Modified: Tue, 21 Dec 2021 07:29:59 GMT  
		Size: 3.8 MB (3806095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d6e9dfd0921d6d978249cbffe7ee768271b9d92e24e4d5bbacf13cae2be2c`  
		Last Modified: Thu, 23 Dec 2021 06:03:06 GMT  
		Size: 112.8 MB (112762993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e8272c9abefc7fc407ef4c323e57bc81ea6ab3fc0f1a43768341030463134faf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145443862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d27d4c12fee754b4473472778584b0492df8f18ad6cebdfa261e0188044ae680`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:52:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:52:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:52:32 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 19:29:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:29:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 19:29:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59091731f7a5e363cc0dd5a19d3e56f18bc4165c020fa2c62a2c23a6a8d55a`  
		Last Modified: Tue, 21 Dec 2021 10:55:14 GMT  
		Size: 4.3 MB (4338189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e878b9f32d144182b2c842e8281a9ef9510213c802f886d0daa2fbae1ca02e1a`  
		Last Modified: Wed, 22 Dec 2021 19:30:50 GMT  
		Size: 115.2 MB (115182524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:772705642a3ec9be6d7537a51953728ed3056cb42338c9cd7fdd58b4e9e2ac7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.7 MB (151684180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539ff53bb81dcd765b491496d29f1897bbc28c84a28b1b5fada0d6a181f65499`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:45:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:45:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:45:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 20:48:00 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 20:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 20:48:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a2d4803cd1b772d17b3feabe820fe1067f750917bf28c21c5d5f468afa7fe8`  
		Last Modified: Tue, 21 Dec 2021 07:49:07 GMT  
		Size: 4.6 MB (4611023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b8fde9629a60fcacb93757ede15e0b99c548233bc76f9500b28ea0cb15fd7`  
		Last Modified: Wed, 22 Dec 2021 20:50:31 GMT  
		Size: 119.3 MB (119268584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore`

```console
$ docker pull julia@sha256:267e263d46e9b6d257129a0270010115dee2aeb99070d253e6d50020a96822fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.6-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:7eea907b57a8580108e6828c9cf2211d605e40560cca8bee98b8debddd81348c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325192216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c112159bff771c5eaaa4dc6c6081da65c73b3eaf80d7791d77dab86ef73614c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:16:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:16:10 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:16:12 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:17:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5bc799d7a6b72fe2a92e227ce3e72eda15852cca648edbffde4f5196b8fd28`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d3a60fc4823edb2dc48e7dc79f2084d47d721aaa552207214459580e2fdd0`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a911a2357de34787001fdca732d87189a8bf1f460da7dab9cdec04b15f583e3b`  
		Last Modified: Wed, 22 Dec 2021 19:24:32 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c27eac142ebf7fc318fb2b32c37051be9434d7f9df6d33107d57c33d670d3`  
		Last Modified: Wed, 22 Dec 2021 19:26:59 GMT  
		Size: 134.4 MB (134413551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07a0883745cb931a41259b2fe70194ae1270f6ed3ab915d79e4ba168a63933e`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:ebfaf0856b165128d116e72cf34bfc013b26d00605d354c951d67f52e93a00dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842770402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a3633b42ac1bb94c430d603bb2248359af77459a0f94be51da03a0e2cdf359`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:18:07 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:18:08 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:18:10 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:20:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec01c86598057b0ba8a30af6624599148001c73b4397623970c17a9b6822c3c`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de51ecc8ca2d4ec960fecf7e7013f4032107c3aa5050d40d8eff7f5d16a831ab`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182ac5c826097666bd787f2234ab9423fb2d2ea72d697ae62d95319efbba475`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4143a01766a217c2a0da621057725e5a229f51c1c8778523f3eea0b04060d`  
		Last Modified: Wed, 22 Dec 2021 19:27:39 GMT  
		Size: 134.2 MB (134158790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a9a3732552b71e088371a52624c70cf32d1d7ed1596cee002b0b248b1cf6d`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:ebf47edb8b2258a6ff50fbf922a30ebf9c40b73fdc18db37c619a1f7c002af62
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408845728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57f595200ff30dcd7b6c90428bcd4aabbe8fb549c3576a48786067f34345172`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:21:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:21:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:21:07 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebef7e05ef5388d95b79785f0dd1f495fa64a0513bf7f2b6eb7b81cc438f93f2`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b69a5c57d23ff9757738234b8d6a6a356a6a07f5e0e2f0c4c62e785b6b54`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb413f4ff9442af4fb91c7ccd16c0aa2e30f45fcc8e56e6c8fd02798416be37`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539c8cb1c574e3ab73950b0c7d634d3dc27dba154c1bcd572ccaed386fa642`  
		Last Modified: Wed, 22 Dec 2021 19:30:18 GMT  
		Size: 134.1 MB (134123877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc8f9569ec24361b165bc28ffb36986ba71988f9f962207c555e6c6c57a714`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:9a27523c78849dffb382d4f7c3c94a6406de56502f386d43c96a62bd9c730b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:ebfaf0856b165128d116e72cf34bfc013b26d00605d354c951d67f52e93a00dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842770402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a3633b42ac1bb94c430d603bb2248359af77459a0f94be51da03a0e2cdf359`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:18:07 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:18:08 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:18:10 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:20:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec01c86598057b0ba8a30af6624599148001c73b4397623970c17a9b6822c3c`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de51ecc8ca2d4ec960fecf7e7013f4032107c3aa5050d40d8eff7f5d16a831ab`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182ac5c826097666bd787f2234ab9423fb2d2ea72d697ae62d95319efbba475`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4143a01766a217c2a0da621057725e5a229f51c1c8778523f3eea0b04060d`  
		Last Modified: Wed, 22 Dec 2021 19:27:39 GMT  
		Size: 134.2 MB (134158790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a9a3732552b71e088371a52624c70cf32d1d7ed1596cee002b0b248b1cf6d`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:f05c7adfb45ae0acf4e9498bd22452ff118783a5764e0ade02ec886e763d9b9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:ebf47edb8b2258a6ff50fbf922a30ebf9c40b73fdc18db37c619a1f7c002af62
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408845728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57f595200ff30dcd7b6c90428bcd4aabbe8fb549c3576a48786067f34345172`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:21:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:21:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:21:07 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebef7e05ef5388d95b79785f0dd1f495fa64a0513bf7f2b6eb7b81cc438f93f2`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b69a5c57d23ff9757738234b8d6a6a356a6a07f5e0e2f0c4c62e785b6b54`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb413f4ff9442af4fb91c7ccd16c0aa2e30f45fcc8e56e6c8fd02798416be37`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539c8cb1c574e3ab73950b0c7d634d3dc27dba154c1bcd572ccaed386fa642`  
		Last Modified: Wed, 22 Dec 2021 19:30:18 GMT  
		Size: 134.1 MB (134123877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc8f9569ec24361b165bc28ffb36986ba71988f9f962207c555e6c6c57a714`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:6bdce73c15736b3674ddab45509c03f80d84d635bae983c0ae5f79f39933a6f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `julia:1.6-windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:7eea907b57a8580108e6828c9cf2211d605e40560cca8bee98b8debddd81348c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325192216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c112159bff771c5eaaa4dc6c6081da65c73b3eaf80d7791d77dab86ef73614c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:16:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:16:10 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:16:12 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:17:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5bc799d7a6b72fe2a92e227ce3e72eda15852cca648edbffde4f5196b8fd28`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d3a60fc4823edb2dc48e7dc79f2084d47d721aaa552207214459580e2fdd0`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a911a2357de34787001fdca732d87189a8bf1f460da7dab9cdec04b15f583e3b`  
		Last Modified: Wed, 22 Dec 2021 19:24:32 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c27eac142ebf7fc318fb2b32c37051be9434d7f9df6d33107d57c33d670d3`  
		Last Modified: Wed, 22 Dec 2021 19:26:59 GMT  
		Size: 134.4 MB (134413551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07a0883745cb931a41259b2fe70194ae1270f6ed3ab915d79e4ba168a63933e`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5`

```console
$ docker pull julia@sha256:60aeb8e45be9ef39f4d9d67c5bb5f8796dcfa11b5b7fc4d2b5aa7c5494e13ded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.6.5` - linux; amd64

```console
$ docker pull julia@sha256:2ef5a0f19f81703f04094c78657b8443e963f7c3b44d6007d0945c7f70bc028a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155401867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5532da26a08b117a16c29c151bb8e13ae160b17f4144bd05707cbf83325e7274`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:58:16 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:58:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 21:58:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38142823e55e64a3bc27c80730299eb1da2984e83f9406ed33ed120d632da445`  
		Last Modified: Wed, 22 Dec 2021 22:00:58 GMT  
		Size: 121.6 MB (121618783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:8311ae235193bfc27bd09087929a37453b4247bf4fa3b56df25c82599e36f08c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141549810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8819044f958a8d0a7bd4db01f03929fb0cd51595a37a0799ccb75aa23ae2249`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:25:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:25:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:25:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:25:43 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Dec 2021 05:58:01 GMT
ENV JULIA_VERSION=1.6.5
# Thu, 23 Dec 2021 05:58:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Dec 2021 05:58:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f37016379049dbd4608d5a4cf9d671487875c1e04a4982557d166d0c5fe138`  
		Last Modified: Tue, 21 Dec 2021 07:28:31 GMT  
		Size: 2.2 MB (2227504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e133e7f3cba6914373c6e9a46ce04ba26872c19a26e94a2e7a1fefd7f17b14`  
		Last Modified: Thu, 23 Dec 2021 06:01:37 GMT  
		Size: 112.8 MB (112761491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a471ad9988b9d589a4ecfc327a6720e6ff716ddfac7cf0b4bd5932eee78d8e9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147627114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c8dea12468b3b39ca9e446a6dcf830516f2a25039d67d670b44b2b423316e2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 19:28:36 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:28:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 19:28:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b6453ae077e7d1f5085e555eccc55c5feeef605098ecb98bbe91c91759d15`  
		Last Modified: Wed, 22 Dec 2021 19:30:22 GMT  
		Size: 115.2 MB (115170876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5` - linux; 386

```console
$ docker pull julia@sha256:ebac08a52e3ba80badffbf207840e27bb1aeba099c25cef49c4c6b488a38e22c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154155382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2f7461565250c49d111ff71d68cdcf7b979d13f410290d287ba7c7b64e5d0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 20:47:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 20:47:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 20:47:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe4f2dda07f20e17a43e7bc704e79462ec5bfc58b4c585d4280450b36ae6d2`  
		Last Modified: Wed, 22 Dec 2021 20:49:50 GMT  
		Size: 119.3 MB (119255036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:7eea907b57a8580108e6828c9cf2211d605e40560cca8bee98b8debddd81348c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325192216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c112159bff771c5eaaa4dc6c6081da65c73b3eaf80d7791d77dab86ef73614c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:16:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:16:10 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:16:12 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:17:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5bc799d7a6b72fe2a92e227ce3e72eda15852cca648edbffde4f5196b8fd28`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d3a60fc4823edb2dc48e7dc79f2084d47d721aaa552207214459580e2fdd0`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a911a2357de34787001fdca732d87189a8bf1f460da7dab9cdec04b15f583e3b`  
		Last Modified: Wed, 22 Dec 2021 19:24:32 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c27eac142ebf7fc318fb2b32c37051be9434d7f9df6d33107d57c33d670d3`  
		Last Modified: Wed, 22 Dec 2021 19:26:59 GMT  
		Size: 134.4 MB (134413551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07a0883745cb931a41259b2fe70194ae1270f6ed3ab915d79e4ba168a63933e`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:ebfaf0856b165128d116e72cf34bfc013b26d00605d354c951d67f52e93a00dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842770402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a3633b42ac1bb94c430d603bb2248359af77459a0f94be51da03a0e2cdf359`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:18:07 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:18:08 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:18:10 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:20:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec01c86598057b0ba8a30af6624599148001c73b4397623970c17a9b6822c3c`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de51ecc8ca2d4ec960fecf7e7013f4032107c3aa5050d40d8eff7f5d16a831ab`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182ac5c826097666bd787f2234ab9423fb2d2ea72d697ae62d95319efbba475`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4143a01766a217c2a0da621057725e5a229f51c1c8778523f3eea0b04060d`  
		Last Modified: Wed, 22 Dec 2021 19:27:39 GMT  
		Size: 134.2 MB (134158790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a9a3732552b71e088371a52624c70cf32d1d7ed1596cee002b0b248b1cf6d`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:ebf47edb8b2258a6ff50fbf922a30ebf9c40b73fdc18db37c619a1f7c002af62
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408845728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57f595200ff30dcd7b6c90428bcd4aabbe8fb549c3576a48786067f34345172`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:21:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:21:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:21:07 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebef7e05ef5388d95b79785f0dd1f495fa64a0513bf7f2b6eb7b81cc438f93f2`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b69a5c57d23ff9757738234b8d6a6a356a6a07f5e0e2f0c4c62e785b6b54`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb413f4ff9442af4fb91c7ccd16c0aa2e30f45fcc8e56e6c8fd02798416be37`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539c8cb1c574e3ab73950b0c7d634d3dc27dba154c1bcd572ccaed386fa642`  
		Last Modified: Wed, 22 Dec 2021 19:30:18 GMT  
		Size: 134.1 MB (134123877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc8f9569ec24361b165bc28ffb36986ba71988f9f962207c555e6c6c57a714`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-alpine`

```console
$ docker pull julia@sha256:9caa4089b61c4ee893ab898cb4c0470d716f714e8a6e616483458770339f81cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.5-alpine` - linux; amd64

```console
$ docker pull julia@sha256:a5b375a5c874d93c0444dbdca526d474a8dc3bd87a00a694273d349bb01c93c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123688600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2c761d44dc029f3d9445e6d6b0c786a67e2bea4d9cfebe39a3847e469099ef`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:59:14 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.5-musl-x86_64.tar.gz'; 			sha256='e38eece6f9f20c7472caf3f8f74a99ad0880921c28e1301461fa7af919880383'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 22 Dec 2021 21:59:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6203055cf397dc97a4889e9a4f7287312c95034ff8f4399131d85e5c14377a1`  
		Last Modified: Wed, 22 Dec 2021 22:01:55 GMT  
		Size: 120.9 MB (120870187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-alpine3.14`

```console
$ docker pull julia@sha256:21f3298f06efc4345863d3794a8473a9afd6bef31fa3c1c1d80230d6c6a98670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.5-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:6a8946aeffb6ea6b7ff18a6e0d039eb1da08415c6496256c782ca58f7f267d93
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123693368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fecc22608b4515475f74e89cd9201c5abf9c0eda7629c3e2c8f7a4fd1026eb8`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:59:37 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.5-musl-x86_64.tar.gz'; 			sha256='e38eece6f9f20c7472caf3f8f74a99ad0880921c28e1301461fa7af919880383'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 22 Dec 2021 21:59:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4463ae12c2ce8489f970877c2f5b1194a28ec4234be9e0ac4adc9bda3500a8`  
		Last Modified: Wed, 22 Dec 2021 22:02:29 GMT  
		Size: 120.9 MB (120870387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-alpine3.15`

```console
$ docker pull julia@sha256:9caa4089b61c4ee893ab898cb4c0470d716f714e8a6e616483458770339f81cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.5-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:a5b375a5c874d93c0444dbdca526d474a8dc3bd87a00a694273d349bb01c93c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123688600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2c761d44dc029f3d9445e6d6b0c786a67e2bea4d9cfebe39a3847e469099ef`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:59:14 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.5-musl-x86_64.tar.gz'; 			sha256='e38eece6f9f20c7472caf3f8f74a99ad0880921c28e1301461fa7af919880383'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 22 Dec 2021 21:59:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6203055cf397dc97a4889e9a4f7287312c95034ff8f4399131d85e5c14377a1`  
		Last Modified: Wed, 22 Dec 2021 22:01:55 GMT  
		Size: 120.9 MB (120870187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-bullseye`

```console
$ docker pull julia@sha256:e2db61d5e0de29272be9bbc6d176eed0e17cb61920b70b8632bcbe458ede283b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.5-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:2ef5a0f19f81703f04094c78657b8443e963f7c3b44d6007d0945c7f70bc028a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155401867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5532da26a08b117a16c29c151bb8e13ae160b17f4144bd05707cbf83325e7274`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:58:16 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:58:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 21:58:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38142823e55e64a3bc27c80730299eb1da2984e83f9406ed33ed120d632da445`  
		Last Modified: Wed, 22 Dec 2021 22:00:58 GMT  
		Size: 121.6 MB (121618783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:8311ae235193bfc27bd09087929a37453b4247bf4fa3b56df25c82599e36f08c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141549810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8819044f958a8d0a7bd4db01f03929fb0cd51595a37a0799ccb75aa23ae2249`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:25:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:25:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:25:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:25:43 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Dec 2021 05:58:01 GMT
ENV JULIA_VERSION=1.6.5
# Thu, 23 Dec 2021 05:58:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Dec 2021 05:58:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f37016379049dbd4608d5a4cf9d671487875c1e04a4982557d166d0c5fe138`  
		Last Modified: Tue, 21 Dec 2021 07:28:31 GMT  
		Size: 2.2 MB (2227504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e133e7f3cba6914373c6e9a46ce04ba26872c19a26e94a2e7a1fefd7f17b14`  
		Last Modified: Thu, 23 Dec 2021 06:01:37 GMT  
		Size: 112.8 MB (112761491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a471ad9988b9d589a4ecfc327a6720e6ff716ddfac7cf0b4bd5932eee78d8e9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147627114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c8dea12468b3b39ca9e446a6dcf830516f2a25039d67d670b44b2b423316e2`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 19:28:36 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:28:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 19:28:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b6453ae077e7d1f5085e555eccc55c5feeef605098ecb98bbe91c91759d15`  
		Last Modified: Wed, 22 Dec 2021 19:30:22 GMT  
		Size: 115.2 MB (115170876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ebac08a52e3ba80badffbf207840e27bb1aeba099c25cef49c4c6b488a38e22c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154155382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2f7461565250c49d111ff71d68cdcf7b979d13f410290d287ba7c7b64e5d0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 20:47:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 20:47:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 20:47:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe4f2dda07f20e17a43e7bc704e79462ec5bfc58b4c585d4280450b36ae6d2`  
		Last Modified: Wed, 22 Dec 2021 20:49:50 GMT  
		Size: 119.3 MB (119255036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-buster`

```console
$ docker pull julia@sha256:ec3c667a63853ae0be71ee4ba759e0cce1ecc5f0382859b70473e39ceb4c48dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:f860e513a73b32a469bbf3e60c41934c9fbf90ae98d458261a5f78925a6794d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153237394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d9c86a8289f9a2582a82c8e869c2433dd85c9597447f5957c92f274f9d5279`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 21:58:50 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 21:59:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 21:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d90b7a76b8623c863a0af16dcdde2098d7b6156e63ae932bae0682bf40db9`  
		Last Modified: Tue, 21 Dec 2021 02:34:37 GMT  
		Size: 4.5 MB (4458501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9a921cde994753f96149f95af939deddcce1eec091151ab4ac295859387671`  
		Last Modified: Wed, 22 Dec 2021 22:01:27 GMT  
		Size: 121.6 MB (121625170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a670efe718cc2152fabacf224bf30ea847c63e6bc1b91d6f76a0408bb3f262c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139323412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b228efb7d262f0b4529e2d9130a2ae5e77b78a108a2c8e5d235087ed77ab7901`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:27:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:27:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:27:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:27:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Dec 2021 05:59:02 GMT
ENV JULIA_VERSION=1.6.5
# Thu, 23 Dec 2021 05:59:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Dec 2021 05:59:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb00b7b6f8221655a7461d12bc7c3eb31d355271d28a924892c78d693001876f`  
		Last Modified: Tue, 21 Dec 2021 07:29:59 GMT  
		Size: 3.8 MB (3806095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d6e9dfd0921d6d978249cbffe7ee768271b9d92e24e4d5bbacf13cae2be2c`  
		Last Modified: Thu, 23 Dec 2021 06:03:06 GMT  
		Size: 112.8 MB (112762993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e8272c9abefc7fc407ef4c323e57bc81ea6ab3fc0f1a43768341030463134faf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145443862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d27d4c12fee754b4473472778584b0492df8f18ad6cebdfa261e0188044ae680`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:52:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:52:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:52:32 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 19:29:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:29:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 19:29:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59091731f7a5e363cc0dd5a19d3e56f18bc4165c020fa2c62a2c23a6a8d55a`  
		Last Modified: Tue, 21 Dec 2021 10:55:14 GMT  
		Size: 4.3 MB (4338189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e878b9f32d144182b2c842e8281a9ef9510213c802f886d0daa2fbae1ca02e1a`  
		Last Modified: Wed, 22 Dec 2021 19:30:50 GMT  
		Size: 115.2 MB (115182524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-buster` - linux; 386

```console
$ docker pull julia@sha256:772705642a3ec9be6d7537a51953728ed3056cb42338c9cd7fdd58b4e9e2ac7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.7 MB (151684180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539ff53bb81dcd765b491496d29f1897bbc28c84a28b1b5fada0d6a181f65499`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:45:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:45:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:45:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 22 Dec 2021 20:48:00 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 20:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.5-linux-x86_64.tar.gz'; 			sha256='b8fe23ee547254a2fe14be587284ed77c78c06c2d8e9aad5febce0d21cab8e2c'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.5-linux-armv7l.tar.gz'; 			sha256='19de0651152aff20feb757f6aa3316d29514e870c3d05ea347c53ba5a44048f0'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.5-linux-aarch64.tar.gz'; 			sha256='5e24d1326ec8590ab382b6836d00f37193ed5198bc115e9c8032cfb71fcf07ba'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.5-linux-i686.tar.gz'; 			sha256='909c275912a9ae4198710e993b388dd1089b8d6279bab74cfab59af2f4d8f38a'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 22 Dec 2021 20:48:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a2d4803cd1b772d17b3feabe820fe1067f750917bf28c21c5d5f468afa7fe8`  
		Last Modified: Tue, 21 Dec 2021 07:49:07 GMT  
		Size: 4.6 MB (4611023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b8fde9629a60fcacb93757ede15e0b99c548233bc76f9500b28ea0cb15fd7`  
		Last Modified: Wed, 22 Dec 2021 20:50:31 GMT  
		Size: 119.3 MB (119268584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-windowsservercore`

```console
$ docker pull julia@sha256:267e263d46e9b6d257129a0270010115dee2aeb99070d253e6d50020a96822fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.6.5-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:7eea907b57a8580108e6828c9cf2211d605e40560cca8bee98b8debddd81348c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325192216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c112159bff771c5eaaa4dc6c6081da65c73b3eaf80d7791d77dab86ef73614c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:16:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:16:10 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:16:12 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:17:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5bc799d7a6b72fe2a92e227ce3e72eda15852cca648edbffde4f5196b8fd28`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d3a60fc4823edb2dc48e7dc79f2084d47d721aaa552207214459580e2fdd0`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a911a2357de34787001fdca732d87189a8bf1f460da7dab9cdec04b15f583e3b`  
		Last Modified: Wed, 22 Dec 2021 19:24:32 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c27eac142ebf7fc318fb2b32c37051be9434d7f9df6d33107d57c33d670d3`  
		Last Modified: Wed, 22 Dec 2021 19:26:59 GMT  
		Size: 134.4 MB (134413551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07a0883745cb931a41259b2fe70194ae1270f6ed3ab915d79e4ba168a63933e`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:ebfaf0856b165128d116e72cf34bfc013b26d00605d354c951d67f52e93a00dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842770402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a3633b42ac1bb94c430d603bb2248359af77459a0f94be51da03a0e2cdf359`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:18:07 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:18:08 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:18:10 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:20:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec01c86598057b0ba8a30af6624599148001c73b4397623970c17a9b6822c3c`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de51ecc8ca2d4ec960fecf7e7013f4032107c3aa5050d40d8eff7f5d16a831ab`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182ac5c826097666bd787f2234ab9423fb2d2ea72d697ae62d95319efbba475`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4143a01766a217c2a0da621057725e5a229f51c1c8778523f3eea0b04060d`  
		Last Modified: Wed, 22 Dec 2021 19:27:39 GMT  
		Size: 134.2 MB (134158790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a9a3732552b71e088371a52624c70cf32d1d7ed1596cee002b0b248b1cf6d`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.5-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:ebf47edb8b2258a6ff50fbf922a30ebf9c40b73fdc18db37c619a1f7c002af62
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408845728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57f595200ff30dcd7b6c90428bcd4aabbe8fb549c3576a48786067f34345172`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:21:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:21:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:21:07 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebef7e05ef5388d95b79785f0dd1f495fa64a0513bf7f2b6eb7b81cc438f93f2`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b69a5c57d23ff9757738234b8d6a6a356a6a07f5e0e2f0c4c62e785b6b54`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb413f4ff9442af4fb91c7ccd16c0aa2e30f45fcc8e56e6c8fd02798416be37`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539c8cb1c574e3ab73950b0c7d634d3dc27dba154c1bcd572ccaed386fa642`  
		Last Modified: Wed, 22 Dec 2021 19:30:18 GMT  
		Size: 134.1 MB (134123877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc8f9569ec24361b165bc28ffb36986ba71988f9f962207c555e6c6c57a714`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:9a27523c78849dffb382d4f7c3c94a6406de56502f386d43c96a62bd9c730b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:1.6.5-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:ebfaf0856b165128d116e72cf34bfc013b26d00605d354c951d67f52e93a00dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842770402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a3633b42ac1bb94c430d603bb2248359af77459a0f94be51da03a0e2cdf359`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:18:07 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:18:08 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:18:10 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:20:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec01c86598057b0ba8a30af6624599148001c73b4397623970c17a9b6822c3c`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de51ecc8ca2d4ec960fecf7e7013f4032107c3aa5050d40d8eff7f5d16a831ab`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182ac5c826097666bd787f2234ab9423fb2d2ea72d697ae62d95319efbba475`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4143a01766a217c2a0da621057725e5a229f51c1c8778523f3eea0b04060d`  
		Last Modified: Wed, 22 Dec 2021 19:27:39 GMT  
		Size: 134.2 MB (134158790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a9a3732552b71e088371a52624c70cf32d1d7ed1596cee002b0b248b1cf6d`  
		Last Modified: Wed, 22 Dec 2021 19:27:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:f05c7adfb45ae0acf4e9498bd22452ff118783a5764e0ade02ec886e763d9b9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:1.6.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:ebf47edb8b2258a6ff50fbf922a30ebf9c40b73fdc18db37c619a1f7c002af62
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408845728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d57f595200ff30dcd7b6c90428bcd4aabbe8fb549c3576a48786067f34345172`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:21:05 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:21:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:21:07 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebef7e05ef5388d95b79785f0dd1f495fa64a0513bf7f2b6eb7b81cc438f93f2`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b0b69a5c57d23ff9757738234b8d6a6a356a6a07f5e0e2f0c4c62e785b6b54`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb413f4ff9442af4fb91c7ccd16c0aa2e30f45fcc8e56e6c8fd02798416be37`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539c8cb1c574e3ab73950b0c7d634d3dc27dba154c1bcd572ccaed386fa642`  
		Last Modified: Wed, 22 Dec 2021 19:30:18 GMT  
		Size: 134.1 MB (134123877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc8f9569ec24361b165bc28ffb36986ba71988f9f962207c555e6c6c57a714`  
		Last Modified: Wed, 22 Dec 2021 19:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.5-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:6bdce73c15736b3674ddab45509c03f80d84d635bae983c0ae5f79f39933a6f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `julia:1.6.5-windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:7eea907b57a8580108e6828c9cf2211d605e40560cca8bee98b8debddd81348c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325192216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c112159bff771c5eaaa4dc6c6081da65c73b3eaf80d7791d77dab86ef73614c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Dec 2021 19:16:09 GMT
ENV JULIA_VERSION=1.6.5
# Wed, 22 Dec 2021 19:16:10 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.5-win64.exe
# Wed, 22 Dec 2021 19:16:12 GMT
ENV JULIA_SHA256=dd2e0404c6ad332b47cfea13796b7826b5d0df0aae6450b976bab8f848bdf948
# Wed, 22 Dec 2021 19:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 22 Dec 2021 19:17:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5bc799d7a6b72fe2a92e227ce3e72eda15852cca648edbffde4f5196b8fd28`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d3a60fc4823edb2dc48e7dc79f2084d47d721aaa552207214459580e2fdd0`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a911a2357de34787001fdca732d87189a8bf1f460da7dab9cdec04b15f583e3b`  
		Last Modified: Wed, 22 Dec 2021 19:24:32 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c27eac142ebf7fc318fb2b32c37051be9434d7f9df6d33107d57c33d670d3`  
		Last Modified: Wed, 22 Dec 2021 19:26:59 GMT  
		Size: 134.4 MB (134413551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07a0883745cb931a41259b2fe70194ae1270f6ed3ab915d79e4ba168a63933e`  
		Last Modified: Wed, 22 Dec 2021 19:24:31 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7`

```console
$ docker pull julia@sha256:545895061073bc6adbae53c0cbe2cac62aa8afd3f204ff745e31d0699969f349
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.7` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-alpine`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.7-alpine` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-alpine3.14`

```console
$ docker pull julia@sha256:8d694f350ed9d13a457d7d33a951594ef7b55cd8a60b5dac116366ffe2fc6920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.7-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:4328442d3c3eb9de31aec772546436b7a9b38ba319a274ad8282e7388c7747c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134595199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5683a72eb9212724b391b9bbe160fecbec5b864b8f7b4432d2d5cf73e75359`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1053bc232f4e5495d158a20c62c5fca1d2b6f2741a93580531bf266910062a8f`  
		Last Modified: Mon, 27 Dec 2021 18:48:49 GMT  
		Size: 131.8 MB (131772218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-alpine3.15`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.7-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-bullseye`

```console
$ docker pull julia@sha256:6bab698fdb707d9988eddac51ec36ec7261e8b2c46510c3769cadd9cc3708729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.7-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7-bullseye` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-buster`

```console
$ docker pull julia@sha256:f0a5766c86b1223bdd91767baa3f3e7c7b914fed37990f9f559ac207d3d88937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.7-buster` - linux; amd64

```console
$ docker pull julia@sha256:8cfa444dfe1e3362b079fbec07fcc7fc47f6061d80425a2c89001e949299bd03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164156514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc405e9ce723306cf702dd4a1a7f29e9caa82c7eb9e908d93382b6c8a9a15733`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:35 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:45:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d90b7a76b8623c863a0af16dcdde2098d7b6156e63ae932bae0682bf40db9`  
		Last Modified: Tue, 21 Dec 2021 02:34:37 GMT  
		Size: 4.5 MB (4458501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a8d66b0aad5d66842ae0e66b6ce78557fee5e7fbc807d1fdb678afe670792`  
		Last Modified: Mon, 27 Dec 2021 18:47:32 GMT  
		Size: 132.5 MB (132544290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:7a4ef7c24e16a63d9a6b8fce489b5359d7ac31e6be2e1fdc78b7f21321714bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155918945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d323828aa7b36c87d276d0dd64eebb7353d57c1965bc6fb36c91793b5bccbe74`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:52:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:52:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:52:32 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:40:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59091731f7a5e363cc0dd5a19d3e56f18bc4165c020fa2c62a2c23a6a8d55a`  
		Last Modified: Tue, 21 Dec 2021 10:55:14 GMT  
		Size: 4.3 MB (4338189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c8ac4ad3e6cbeda7573be619cb77e0c983ee2038d4ed72440cb59f763cec4e`  
		Last Modified: Mon, 27 Dec 2021 17:42:34 GMT  
		Size: 125.7 MB (125657607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7-buster` - linux; 386

```console
$ docker pull julia@sha256:d96339edf04f747dbb364f9c34c616341d65ea9aefa14a7936f1c8ef7fd59fbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161209682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9195370cc3121df2b7f9aac958404af4c50c8c904cc72ab039807c49280eac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:45:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:45:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:45:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:17 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a2d4803cd1b772d17b3feabe820fe1067f750917bf28c21c5d5f468afa7fe8`  
		Last Modified: Tue, 21 Dec 2021 07:49:07 GMT  
		Size: 4.6 MB (4611023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad77c239750f92c468b5b65093a40d17fec6cb412e71a13ec5d250b728bf666`  
		Last Modified: Mon, 27 Dec 2021 17:41:45 GMT  
		Size: 128.8 MB (128794086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-windowsservercore`

```console
$ docker pull julia@sha256:cade52ef6d84e8447cc04650915a7076ee9bdb9b945bcae2a2ed6d559664742a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.7-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-windowsservercore-1809`

```console
$ docker pull julia@sha256:0ec7efc01d8fe5085ffeca6137c838136653f2ccabb9e559673f6c434d5fdb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:1.7-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:1fefcc3c73f90296644ee58bcb1046c76116e0f5604ba82b78c8c8e3c2b648ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:1.7-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:f02889aee8ceaab805f4b9379afe9a4f15e3ef86313a305cd66c143b1b13626c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `julia:1.7-windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1`

```console
$ docker pull julia@sha256:545895061073bc6adbae53c0cbe2cac62aa8afd3f204ff745e31d0699969f349
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.7.1` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-alpine`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.7.1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-alpine3.14`

```console
$ docker pull julia@sha256:8d694f350ed9d13a457d7d33a951594ef7b55cd8a60b5dac116366ffe2fc6920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.7.1-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:4328442d3c3eb9de31aec772546436b7a9b38ba319a274ad8282e7388c7747c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134595199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5683a72eb9212724b391b9bbe160fecbec5b864b8f7b4432d2d5cf73e75359`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1053bc232f4e5495d158a20c62c5fca1d2b6f2741a93580531bf266910062a8f`  
		Last Modified: Mon, 27 Dec 2021 18:48:49 GMT  
		Size: 131.8 MB (131772218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-alpine3.15`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.7.1-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-bullseye`

```console
$ docker pull julia@sha256:6bab698fdb707d9988eddac51ec36ec7261e8b2c46510c3769cadd9cc3708729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.7.1-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1-bullseye` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-buster`

```console
$ docker pull julia@sha256:f0a5766c86b1223bdd91767baa3f3e7c7b914fed37990f9f559ac207d3d88937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.7.1-buster` - linux; amd64

```console
$ docker pull julia@sha256:8cfa444dfe1e3362b079fbec07fcc7fc47f6061d80425a2c89001e949299bd03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164156514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc405e9ce723306cf702dd4a1a7f29e9caa82c7eb9e908d93382b6c8a9a15733`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:35 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:45:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d90b7a76b8623c863a0af16dcdde2098d7b6156e63ae932bae0682bf40db9`  
		Last Modified: Tue, 21 Dec 2021 02:34:37 GMT  
		Size: 4.5 MB (4458501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a8d66b0aad5d66842ae0e66b6ce78557fee5e7fbc807d1fdb678afe670792`  
		Last Modified: Mon, 27 Dec 2021 18:47:32 GMT  
		Size: 132.5 MB (132544290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:7a4ef7c24e16a63d9a6b8fce489b5359d7ac31e6be2e1fdc78b7f21321714bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155918945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d323828aa7b36c87d276d0dd64eebb7353d57c1965bc6fb36c91793b5bccbe74`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:52:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:52:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:52:32 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:40:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59091731f7a5e363cc0dd5a19d3e56f18bc4165c020fa2c62a2c23a6a8d55a`  
		Last Modified: Tue, 21 Dec 2021 10:55:14 GMT  
		Size: 4.3 MB (4338189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c8ac4ad3e6cbeda7573be619cb77e0c983ee2038d4ed72440cb59f763cec4e`  
		Last Modified: Mon, 27 Dec 2021 17:42:34 GMT  
		Size: 125.7 MB (125657607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1-buster` - linux; 386

```console
$ docker pull julia@sha256:d96339edf04f747dbb364f9c34c616341d65ea9aefa14a7936f1c8ef7fd59fbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161209682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9195370cc3121df2b7f9aac958404af4c50c8c904cc72ab039807c49280eac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:45:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:45:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:45:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:17 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a2d4803cd1b772d17b3feabe820fe1067f750917bf28c21c5d5f468afa7fe8`  
		Last Modified: Tue, 21 Dec 2021 07:49:07 GMT  
		Size: 4.6 MB (4611023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad77c239750f92c468b5b65093a40d17fec6cb412e71a13ec5d250b728bf666`  
		Last Modified: Mon, 27 Dec 2021 17:41:45 GMT  
		Size: 128.8 MB (128794086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-windowsservercore`

```console
$ docker pull julia@sha256:cade52ef6d84e8447cc04650915a7076ee9bdb9b945bcae2a2ed6d559664742a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:1.7.1-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.7.1-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-windowsservercore-1809`

```console
$ docker pull julia@sha256:0ec7efc01d8fe5085ffeca6137c838136653f2ccabb9e559673f6c434d5fdb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:1.7.1-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:1fefcc3c73f90296644ee58bcb1046c76116e0f5604ba82b78c8c8e3c2b648ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:1.7.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.7.1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:f02889aee8ceaab805f4b9379afe9a4f15e3ef86313a305cd66c143b1b13626c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `julia:1.7.1-windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.14`

```console
$ docker pull julia@sha256:8d694f350ed9d13a457d7d33a951594ef7b55cd8a60b5dac116366ffe2fc6920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:4328442d3c3eb9de31aec772546436b7a9b38ba319a274ad8282e7388c7747c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134595199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5683a72eb9212724b391b9bbe160fecbec5b864b8f7b4432d2d5cf73e75359`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1053bc232f4e5495d158a20c62c5fca1d2b6f2741a93580531bf266910062a8f`  
		Last Modified: Mon, 27 Dec 2021 18:48:49 GMT  
		Size: 131.8 MB (131772218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.15`

```console
$ docker pull julia@sha256:fb37a8218f4dd27e42fc9d28aff2b7d69d9a312cd46073c4272d9a85b0df8dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:4f06670d440e698b3356d3efb5d9c967c516994b9056d27f0c884f09b1f370d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134590425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a25cc154661e0dc037298fbdf70e7233449a8c3a595fa07ce6ce99b79920055`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:03 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c344de3082b3171b02d6a10c284311a8373deaab68448c5dc0286e22bfad46e`  
		Last Modified: Mon, 27 Dec 2021 18:48:06 GMT  
		Size: 131.8 MB (131772012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:bullseye`

```console
$ docker pull julia@sha256:6bab698fdb707d9988eddac51ec36ec7261e8b2c46510c3769cadd9cc3708729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:bullseye` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:f0a5766c86b1223bdd91767baa3f3e7c7b914fed37990f9f559ac207d3d88937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:8cfa444dfe1e3362b079fbec07fcc7fc47f6061d80425a2c89001e949299bd03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164156514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc405e9ce723306cf702dd4a1a7f29e9caa82c7eb9e908d93382b6c8a9a15733`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:35 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:45:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d90b7a76b8623c863a0af16dcdde2098d7b6156e63ae932bae0682bf40db9`  
		Last Modified: Tue, 21 Dec 2021 02:34:37 GMT  
		Size: 4.5 MB (4458501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a8d66b0aad5d66842ae0e66b6ce78557fee5e7fbc807d1fdb678afe670792`  
		Last Modified: Mon, 27 Dec 2021 18:47:32 GMT  
		Size: 132.5 MB (132544290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:7a4ef7c24e16a63d9a6b8fce489b5359d7ac31e6be2e1fdc78b7f21321714bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155918945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d323828aa7b36c87d276d0dd64eebb7353d57c1965bc6fb36c91793b5bccbe74`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:52:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:52:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:52:32 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:40:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59091731f7a5e363cc0dd5a19d3e56f18bc4165c020fa2c62a2c23a6a8d55a`  
		Last Modified: Tue, 21 Dec 2021 10:55:14 GMT  
		Size: 4.3 MB (4338189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c8ac4ad3e6cbeda7573be619cb77e0c983ee2038d4ed72440cb59f763cec4e`  
		Last Modified: Mon, 27 Dec 2021 17:42:34 GMT  
		Size: 125.7 MB (125657607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:d96339edf04f747dbb364f9c34c616341d65ea9aefa14a7936f1c8ef7fd59fbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161209682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9195370cc3121df2b7f9aac958404af4c50c8c904cc72ab039807c49280eac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:45:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:45:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:45:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:17 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a2d4803cd1b772d17b3feabe820fe1067f750917bf28c21c5d5f468afa7fe8`  
		Last Modified: Tue, 21 Dec 2021 07:49:07 GMT  
		Size: 4.6 MB (4611023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad77c239750f92c468b5b65093a40d17fec6cb412e71a13ec5d250b728bf666`  
		Last Modified: Mon, 27 Dec 2021 17:41:45 GMT  
		Size: 128.8 MB (128794086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:545895061073bc6adbae53c0cbe2cac62aa8afd3f204ff745e31d0699969f349
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:4f71e0d52199bd7b6b9e23e7ac4575aa147f7f040884c7261c5bba93b4ef2f94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166334774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a71ad60d549b6f16ec989a10711214b904c09a15526c052fd4ceb024268221`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 02:30:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:30:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:44:07 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 18:44:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d5e20d588d9a869aa25ce8aba77d1a7796193dc38a36b69b55074b24e87c`  
		Last Modified: Tue, 21 Dec 2021 02:33:57 GMT  
		Size: 2.4 MB (2425460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531289aa620a61ac049947cc184f2bfa511334ea6e54c3ba36049a04aa9aebce`  
		Last Modified: Mon, 27 Dec 2021 18:46:58 GMT  
		Size: 132.6 MB (132551690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:71e8011f928e9525de767ecf59dc6b971a4aa202b3203d8bf6717fd85df188c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158117917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb6e21c911993b152d6455f1f98e422b5446e641078197721cc55e56edd3607`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:51:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:51:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 10:51:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 10:51:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:39:54 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:40:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:40:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b034c4ff086209d57d33db1856d203c19c51bcc27801df1303385f9c8dfac6b`  
		Last Modified: Tue, 21 Dec 2021 10:54:36 GMT  
		Size: 2.4 MB (2412445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec0ff7b8e8a8280373de58608b24b66752880ea2929310cbb416205140bac6`  
		Last Modified: Mon, 27 Dec 2021 17:41:59 GMT  
		Size: 125.7 MB (125661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:df76aeac04a0005a7224c3283ac4c020c11823fbc4aa3c6b08b10c50811ad5c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163684118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3a96591d4c6d611d2b5f2a80058749cb3b0f7adf1f93f9fe1bd729ac9d1178`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:44:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:44:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 21 Dec 2021 07:44:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 07:44:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 17:38:41 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 17:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.1-linux-x86_64.tar.gz'; 			sha256='44658e9c7b45e2b9b5b59239d190cca42de05c175ea86bc346c294a8fe8d9f11'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.1-linux-aarch64.tar.gz'; 			sha256='5d9f23916d331f54a2bb68936c2c7fbf3fdb4a6f7bfbb99750276cc23a292a4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.1-linux-i686.tar.gz'; 			sha256='6b5f7a235dc51b586d6ab914042b6d91c8634eeeb011636460ab6dcbf5671fac'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 27 Dec 2021 17:39:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fcb5545b246aed9c9865e6d387c4698008abdd695e268ab79f090186bc2f34`  
		Last Modified: Tue, 21 Dec 2021 07:48:03 GMT  
		Size: 2.5 MB (2529496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42295fc33b55df0c57d4d437c689e6d6fa126c60f161673bca5b34cc8e82326`  
		Last Modified: Mon, 27 Dec 2021 17:41:03 GMT  
		Size: 128.8 MB (128783772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore`

```console
$ docker pull julia@sha256:cade52ef6d84e8447cc04650915a7076ee9bdb9b945bcae2a2ed6d559664742a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `julia:windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:0ec7efc01d8fe5085ffeca6137c838136653f2ccabb9e559673f6c434d5fdb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:1fefcc3c73f90296644ee58bcb1046c76116e0f5604ba82b78c8c8e3c2b648ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:6502dd1f8ab57b85a3b7ccddf7baa81ccd9b988564afc600dc74765d0b749a93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf671754e05f5235a2448c04a383964e668cca9e2f76e3743be60b182ca53ba9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:21:04 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:21:05 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:21:06 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:24:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:24:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8205087253930ad49201926a5502e63bb90c70728500021cc5e94aa118f005`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065385d2d3b2724fff4cd1d5400f5294e1a141fb066f27637abc5464299b6be3`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270f612fb3874b118735419b76b9bc54cb8270e2faf2bd1614b79119ff0adb`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97264b37e21836da29811f28dad3029a6c6e94204af3dc495cc2eb59f12e9f8e`  
		Last Modified: Mon, 27 Dec 2021 18:29:19 GMT  
		Size: 144.7 MB (144664807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a1b27656a36dd7cebfed95233ea398d8729507c203748bcf1ddf32eaddc1`  
		Last Modified: Mon, 27 Dec 2021 18:28:47 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:f02889aee8ceaab805f4b9379afe9a4f15e3ef86313a305cd66c143b1b13626c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `julia:windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

```console
$ docker pull julia@sha256:54b0af6e73635cd3c19325151c9162116970a5c8cadf1c258831ab8dd252e145
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2335746123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51603bd0b8d739c50a2d5623bde2213bb4600664bd082f9a8f265eeefd600bc9`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:15:30 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:15:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:15:32 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:17:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:17:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340a05917c6b7a9123dfd72874e5f771906b937670ca132d25f565e6f0ebde5`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d25e87be4a8dca2d609feb380f7844ccf1d4736693320665441094db34047c`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a907e558555643985dde3728a13fc3eb86af6547138683bd415c05691f33b399`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b197b105480ef217be38efde4b166f367862a9e5475ee093a9df05af91fcd019`  
		Last Modified: Mon, 27 Dec 2021 18:27:47 GMT  
		Size: 145.0 MB (144967508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d0f78bff9e5009d932796cdaa777ed4e142ccdc7a4a6b7001f334efaf1f6d`  
		Last Modified: Mon, 27 Dec 2021 18:25:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
