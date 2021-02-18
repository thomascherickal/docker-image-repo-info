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
-	[`julia:1.5`](#julia15)
-	[`julia:1.5.3`](#julia153)
-	[`julia:1.5.3-alpine`](#julia153-alpine)
-	[`julia:1.5.3-alpine3.12`](#julia153-alpine312)
-	[`julia:1.5.3-alpine3.13`](#julia153-alpine313)
-	[`julia:1.5.3-buster`](#julia153-buster)
-	[`julia:1.5.3-windowsservercore-1809`](#julia153-windowsservercore-1809)
-	[`julia:1.5.3-windowsservercore-ltsc2016`](#julia153-windowsservercore-ltsc2016)
-	[`julia:1.5-alpine`](#julia15-alpine)
-	[`julia:1.5-alpine3.12`](#julia15-alpine312)
-	[`julia:1.5-alpine3.13`](#julia15-alpine313)
-	[`julia:1.5-buster`](#julia15-buster)
-	[`julia:1.5-windowsservercore-1809`](#julia15-windowsservercore-1809)
-	[`julia:1.5-windowsservercore-ltsc2016`](#julia15-windowsservercore-ltsc2016)
-	[`julia:1.6`](#julia16)
-	[`julia:1.6.0`](#julia160)
-	[`julia:1.6.0-buster`](#julia160-buster)
-	[`julia:1.6.0-rc1`](#julia160-rc1)
-	[`julia:1.6.0-rc1-buster`](#julia160-rc1-buster)
-	[`julia:1.6.0-rc1-windowsservercore-1809`](#julia160-rc1-windowsservercore-1809)
-	[`julia:1.6.0-rc1-windowsservercore-ltsc2016`](#julia160-rc1-windowsservercore-ltsc2016)
-	[`julia:1.6.0-windowsservercore-1809`](#julia160-windowsservercore-1809)
-	[`julia:1.6.0-windowsservercore-ltsc2016`](#julia160-windowsservercore-ltsc2016)
-	[`julia:1.6-buster`](#julia16-buster)
-	[`julia:1.6-rc`](#julia16-rc)
-	[`julia:1.6-rc-buster`](#julia16-rc-buster)
-	[`julia:1.6-rc-windowsservercore-1809`](#julia16-rc-windowsservercore-1809)
-	[`julia:1.6-rc-windowsservercore-ltsc2016`](#julia16-rc-windowsservercore-ltsc2016)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2016`](#julia16-windowsservercore-ltsc2016)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.12`](#julia1-alpine312)
-	[`julia:1-alpine3.13`](#julia1-alpine313)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2016`](#julia1-windowsservercore-ltsc2016)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.12`](#juliaalpine312)
-	[`julia:alpine3.13`](#juliaalpine313)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)

## `julia:1`

```console
$ docker pull julia@sha256:e7a4cb833d3078a68c4935e738d7b199c732ec0b120ce2c5fecc6e6d826bd318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:abc78e9eee0a44855691d95424a7050b67bfde76bcad3c261b28ae0d35943b50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:3a0dcd2f281e33c06d3ab63e83c70f7db0707937086868572024be2a7b52571d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127114363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eeacc6fa505e4d7312ffe842835f862af91646d6f1a1e0b828491ba7226f55`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:56 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 05:37:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:37:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2c19f8b85141b684b72ac838636372e568b01834e0cf5f1d0a9047b78e812`  
		Last Modified: Tue, 09 Feb 2021 05:40:21 GMT  
		Size: 95.6 MB (95563283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a8b1a0b46c88bc657c7049e0c977e83a294ba6da409e6da761f249d45a44cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113637324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4260e576eb779ff1b76d80373840d57feaa8fd580ab8510856854d7a03c8d1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:16:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:16:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 03:16:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 03:16:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 03:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 05:57:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 Feb 2021 05:57:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa219c983dff4f994e3a40eea7fe79b5cd8a401e095739cbcd515ef8513d078e`  
		Last Modified: Wed, 10 Feb 2021 05:58:43 GMT  
		Size: 3.8 MB (3804985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dd26452211bcf516ca9f4107f957017daa51834da7a18a386c53d71268f5dc`  
		Last Modified: Wed, 10 Feb 2021 05:59:11 GMT  
		Size: 87.1 MB (87128955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:554976c882252a014a151b7c06f499d7fd16fa867c461d4ad2da18a2feb55cf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110080393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f5f4c9d83020d090072c26ea47bdcdd3df372068f1e87d82d88d4e78c40ce6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:55:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 21:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:45:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c57aa437368cc78c67a8620d603f7b68778ebb227bd03a0a224d8fdf4aa488`  
		Last Modified: Tue, 09 Feb 2021 21:47:49 GMT  
		Size: 79.9 MB (79891106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:44cf61067e705e9f63790812f57a969d3e6dd8ad73e20c46aa93260ce78b34b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124860461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e74523be1d2ea57360b0af349ccbbfed50100c365f860c2fd920e325f413163`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 20:16:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bbec1829f62fe14d3a012d6c128c3ccf39cbe18cdc6ec5113c9ab8a6194dee`  
		Last Modified: Tue, 09 Feb 2021 20:19:49 GMT  
		Size: 92.5 MB (92498680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:7cfd05f41e80511f98c789ab39eabbe40eb165cfc9f9048bdd2bbb69f126d090
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2546632000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4cbed689a02455eb3f26430cf502ff411c96e37869da13b0ea15f239a626b0`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:42:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:42:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c26da75e3692d075b8cc90f8e94e256478a20d09583dfb783167e2e0380194`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b98a5d75905f2eb4b3d70be1fe0d098358b64e50950c012cb9ecb05b3cfcecf`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451757b457dda2cb3a548462583261fb227d9adbca6abb5f1e2e952447e08431`  
		Last Modified: Wed, 10 Feb 2021 15:57:22 GMT  
		Size: 107.4 MB (107359734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa29bf77fc353bbde6f8398ea82e6863560e775323cdb11e6f8816ccb0055e9`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:a043552752781077d5904fa96e3f394cb5d6e65f79e8b703e4af6188706e5c6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5903136908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66bfb21c71c4413d6a9ea1b509fec68b8ffe64d94698d3d8b7fd317dcbdd9eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:43:00 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:43:01 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:45:01 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:45:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf04a1bf70bc380723778f6b70ecc31a982c47090c0b72d56c1d534b6614c6`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54410ac5d0ad2c510f83f9d4cf7a5f393fd7e678ece07106faa2e90ff9473131`  
		Last Modified: Wed, 10 Feb 2021 15:57:35 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167063bef9cef158705c6ef5ae1f7576970568e6d06f95fd3fb89c45f5f9b654`  
		Last Modified: Wed, 10 Feb 2021 15:59:40 GMT  
		Size: 108.1 MB (108118430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeebbf24fc2c457e5491930a59cf8b87672aed1070138e3f42cc40d9520a199`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:abc78e9eee0a44855691d95424a7050b67bfde76bcad3c261b28ae0d35943b50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:3a0dcd2f281e33c06d3ab63e83c70f7db0707937086868572024be2a7b52571d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127114363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eeacc6fa505e4d7312ffe842835f862af91646d6f1a1e0b828491ba7226f55`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:56 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 05:37:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:37:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2c19f8b85141b684b72ac838636372e568b01834e0cf5f1d0a9047b78e812`  
		Last Modified: Tue, 09 Feb 2021 05:40:21 GMT  
		Size: 95.6 MB (95563283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a8b1a0b46c88bc657c7049e0c977e83a294ba6da409e6da761f249d45a44cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113637324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4260e576eb779ff1b76d80373840d57feaa8fd580ab8510856854d7a03c8d1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:16:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:16:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 03:16:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 03:16:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 03:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 05:57:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 Feb 2021 05:57:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa219c983dff4f994e3a40eea7fe79b5cd8a401e095739cbcd515ef8513d078e`  
		Last Modified: Wed, 10 Feb 2021 05:58:43 GMT  
		Size: 3.8 MB (3804985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dd26452211bcf516ca9f4107f957017daa51834da7a18a386c53d71268f5dc`  
		Last Modified: Wed, 10 Feb 2021 05:59:11 GMT  
		Size: 87.1 MB (87128955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:554976c882252a014a151b7c06f499d7fd16fa867c461d4ad2da18a2feb55cf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110080393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f5f4c9d83020d090072c26ea47bdcdd3df372068f1e87d82d88d4e78c40ce6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:55:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 21:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:45:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c57aa437368cc78c67a8620d603f7b68778ebb227bd03a0a224d8fdf4aa488`  
		Last Modified: Tue, 09 Feb 2021 21:47:49 GMT  
		Size: 79.9 MB (79891106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:44cf61067e705e9f63790812f57a969d3e6dd8ad73e20c46aa93260ce78b34b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124860461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e74523be1d2ea57360b0af349ccbbfed50100c365f860c2fd920e325f413163`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 20:16:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bbec1829f62fe14d3a012d6c128c3ccf39cbe18cdc6ec5113c9ab8a6194dee`  
		Last Modified: Tue, 09 Feb 2021 20:19:49 GMT  
		Size: 92.5 MB (92498680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:7cfd05f41e80511f98c789ab39eabbe40eb165cfc9f9048bdd2bbb69f126d090
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2546632000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4cbed689a02455eb3f26430cf502ff411c96e37869da13b0ea15f239a626b0`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:42:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:42:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c26da75e3692d075b8cc90f8e94e256478a20d09583dfb783167e2e0380194`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b98a5d75905f2eb4b3d70be1fe0d098358b64e50950c012cb9ecb05b3cfcecf`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451757b457dda2cb3a548462583261fb227d9adbca6abb5f1e2e952447e08431`  
		Last Modified: Wed, 10 Feb 2021 15:57:22 GMT  
		Size: 107.4 MB (107359734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa29bf77fc353bbde6f8398ea82e6863560e775323cdb11e6f8816ccb0055e9`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:a043552752781077d5904fa96e3f394cb5d6e65f79e8b703e4af6188706e5c6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5903136908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66bfb21c71c4413d6a9ea1b509fec68b8ffe64d94698d3d8b7fd317dcbdd9eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:43:00 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:43:01 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:45:01 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:45:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf04a1bf70bc380723778f6b70ecc31a982c47090c0b72d56c1d534b6614c6`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54410ac5d0ad2c510f83f9d4cf7a5f393fd7e678ece07106faa2e90ff9473131`  
		Last Modified: Wed, 10 Feb 2021 15:57:35 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167063bef9cef158705c6ef5ae1f7576970568e6d06f95fd3fb89c45f5f9b654`  
		Last Modified: Wed, 10 Feb 2021 15:59:40 GMT  
		Size: 108.1 MB (108118430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeebbf24fc2c457e5491930a59cf8b87672aed1070138e3f42cc40d9520a199`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:97784656aa7b73642ae245bec331519f9263350349296bdc27b38bc27b2d57b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:3a0dcd2f281e33c06d3ab63e83c70f7db0707937086868572024be2a7b52571d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127114363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eeacc6fa505e4d7312ffe842835f862af91646d6f1a1e0b828491ba7226f55`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:56 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 05:37:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:37:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2c19f8b85141b684b72ac838636372e568b01834e0cf5f1d0a9047b78e812`  
		Last Modified: Tue, 09 Feb 2021 05:40:21 GMT  
		Size: 95.6 MB (95563283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a8b1a0b46c88bc657c7049e0c977e83a294ba6da409e6da761f249d45a44cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113637324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4260e576eb779ff1b76d80373840d57feaa8fd580ab8510856854d7a03c8d1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:16:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:16:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 03:16:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 03:16:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 03:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 05:57:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 Feb 2021 05:57:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa219c983dff4f994e3a40eea7fe79b5cd8a401e095739cbcd515ef8513d078e`  
		Last Modified: Wed, 10 Feb 2021 05:58:43 GMT  
		Size: 3.8 MB (3804985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dd26452211bcf516ca9f4107f957017daa51834da7a18a386c53d71268f5dc`  
		Last Modified: Wed, 10 Feb 2021 05:59:11 GMT  
		Size: 87.1 MB (87128955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:554976c882252a014a151b7c06f499d7fd16fa867c461d4ad2da18a2feb55cf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110080393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f5f4c9d83020d090072c26ea47bdcdd3df372068f1e87d82d88d4e78c40ce6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:55:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 21:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:45:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c57aa437368cc78c67a8620d603f7b68778ebb227bd03a0a224d8fdf4aa488`  
		Last Modified: Tue, 09 Feb 2021 21:47:49 GMT  
		Size: 79.9 MB (79891106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:44cf61067e705e9f63790812f57a969d3e6dd8ad73e20c46aa93260ce78b34b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124860461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e74523be1d2ea57360b0af349ccbbfed50100c365f860c2fd920e325f413163`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 20:16:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bbec1829f62fe14d3a012d6c128c3ccf39cbe18cdc6ec5113c9ab8a6194dee`  
		Last Modified: Tue, 09 Feb 2021 20:19:49 GMT  
		Size: 92.5 MB (92498680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:511d712d1f83a691ce96eb4f6cabc89a6012024a0b6f73f4de5db048a2d24768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:a8cf8095c224b4149e40344a2c9b5ab7662dd2d5d28f892f62f3f7474faea8bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150421960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f75dc03bb02073b06ed205f78d93864e77d0c97cf0ab4b89ff7e96955f51ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:37:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:37:36 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:37:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aff8b3c8cd719f99f940db3d69b9fdfd832dd1b472dab3cae6a3c5e0b6c291`  
		Last Modified: Tue, 09 Feb 2021 05:40:30 GMT  
		Size: 9.5 MB (9468394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0dc90c59f637f8c9d4f63c0a15bc869fe6405d52b19c37f47cf124f0c8c1da`  
		Last Modified: Tue, 09 Feb 2021 05:40:52 GMT  
		Size: 95.6 MB (95573681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:d8cef96661ca3b7a3f525ad90822c27b851fa5b889c2852aafe890224f619c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137443966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34499f98ea14274e201fee8cc738caab87934be61b8b2011e1b312b36a698bf`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 03:04:53 GMT
ADD file:f884b9fc23d1b8ad0bd21aa823afd0ee186bdebb6829ccba72f77caaeffd8d12 in / 
# Tue, 09 Feb 2021 03:04:55 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:17:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:17:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 03:17:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 03:17:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 03:17:18 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 05:58:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 Feb 2021 05:58:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5275c778c803ce7d82407c77cfad4fb07fd1ec80fc99ba94cef475a92e4d090c`  
		Last Modified: Tue, 09 Feb 2021 03:13:25 GMT  
		Size: 42.1 MB (42119892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33724ddfadc9df78f13b323674fdbf73e45f1d5096c0bce41f2d1fd9808019ff`  
		Last Modified: Wed, 10 Feb 2021 05:59:23 GMT  
		Size: 8.2 MB (8186473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea525324e712b7bdb3b2588fc9a27f73316246cee0c671d9a80ba668b64ce19`  
		Last Modified: Wed, 10 Feb 2021 05:59:47 GMT  
		Size: 87.1 MB (87137601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:81a289e1eeb92cfc09030a575ff664aa73b1bce223fab7a6a861e331079d33c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131523488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf9c3d4c205bd0fa72b56d6f58f8edae1293069d4818bb4040a7d1beee416aa`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:17 GMT
ADD file:fb69ff7b2a28f793efbd16e04b74ffb4557d39e1844b3789075b4d3ff97a0eaa in / 
# Tue, 09 Feb 2021 02:43:20 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:56:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:56:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:56:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:56:47 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 21:45:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:45:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:296c9f0bf5f2cf24e87bc5abd674fc486e8df419d4aa2d362453f64d38900504`  
		Last Modified: Tue, 09 Feb 2021 02:49:43 GMT  
		Size: 43.2 MB (43177550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65852c032a65dbd4a864997474741aff544a12e280cbd00b2b24755d862e19c7`  
		Last Modified: Tue, 09 Feb 2021 21:48:00 GMT  
		Size: 8.4 MB (8437015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e99d810313916e7e4e61ffa7ef5c000c1e6c6ddc2f115aa94fc4d55bdb2f58`  
		Last Modified: Tue, 09 Feb 2021 21:48:19 GMT  
		Size: 79.9 MB (79908923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:038fa0c0ce37234a69160e2841fe0938896f3a1f74879363feb5f94b96678dae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148073769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684ba79f7e666db1fe1dc39fa60c57933b0a83d7044c3202cc642e5dc8232e74`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:08 GMT
ADD file:4c25bc56152d0955bbdef26f612b172a90484913cbd1ab3332b3444c8c0c012e in / 
# Tue, 09 Feb 2021 02:42:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:17:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:17:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:17:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:17:05 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 20:17:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:17:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5d7d8e56e51b8663a269c93107dcdf848d2f6a4f73ca51bb1ced208a1fa80c32`  
		Last Modified: Tue, 09 Feb 2021 02:49:23 GMT  
		Size: 46.1 MB (46097671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5fa89c1a6d759481e9dd18bf72ced3caf53e79be2ef6a132ac2a0115efb9b7`  
		Last Modified: Tue, 09 Feb 2021 20:19:57 GMT  
		Size: 9.5 MB (9474535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7a1c4781aa3b037108e1ec041dfbe9a58e7ae602497cb4696d0e9cddff0c47`  
		Last Modified: Tue, 09 Feb 2021 20:20:20 GMT  
		Size: 92.5 MB (92501563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:87795369570c665c79864d9b91ffda053404284522a00c670553ca9597722b8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.0.5-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:7cfd05f41e80511f98c789ab39eabbe40eb165cfc9f9048bdd2bbb69f126d090
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2546632000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4cbed689a02455eb3f26430cf502ff411c96e37869da13b0ea15f239a626b0`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:42:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:42:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c26da75e3692d075b8cc90f8e94e256478a20d09583dfb783167e2e0380194`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b98a5d75905f2eb4b3d70be1fe0d098358b64e50950c012cb9ecb05b3cfcecf`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451757b457dda2cb3a548462583261fb227d9adbca6abb5f1e2e952447e08431`  
		Last Modified: Wed, 10 Feb 2021 15:57:22 GMT  
		Size: 107.4 MB (107359734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa29bf77fc353bbde6f8398ea82e6863560e775323cdb11e6f8816ccb0055e9`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:56c498b1c25d34165af969da8c0c0bf1a5ec739dbbc1f5b21e8992a296ff3972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:a043552752781077d5904fa96e3f394cb5d6e65f79e8b703e4af6188706e5c6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5903136908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66bfb21c71c4413d6a9ea1b509fec68b8ffe64d94698d3d8b7fd317dcbdd9eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:43:00 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:43:01 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:45:01 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:45:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf04a1bf70bc380723778f6b70ecc31a982c47090c0b72d56c1d534b6614c6`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54410ac5d0ad2c510f83f9d4cf7a5f393fd7e678ece07106faa2e90ff9473131`  
		Last Modified: Wed, 10 Feb 2021 15:57:35 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167063bef9cef158705c6ef5ae1f7576970568e6d06f95fd3fb89c45f5f9b654`  
		Last Modified: Wed, 10 Feb 2021 15:59:40 GMT  
		Size: 108.1 MB (108118430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeebbf24fc2c457e5491930a59cf8b87672aed1070138e3f42cc40d9520a199`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:97784656aa7b73642ae245bec331519f9263350349296bdc27b38bc27b2d57b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:3a0dcd2f281e33c06d3ab63e83c70f7db0707937086868572024be2a7b52571d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127114363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eeacc6fa505e4d7312ffe842835f862af91646d6f1a1e0b828491ba7226f55`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:56 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 05:37:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:37:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b2c19f8b85141b684b72ac838636372e568b01834e0cf5f1d0a9047b78e812`  
		Last Modified: Tue, 09 Feb 2021 05:40:21 GMT  
		Size: 95.6 MB (95563283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8a8b1a0b46c88bc657c7049e0c977e83a294ba6da409e6da761f249d45a44cc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113637324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4260e576eb779ff1b76d80373840d57feaa8fd580ab8510856854d7a03c8d1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:16:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:16:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 03:16:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 03:16:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 03:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 05:57:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 Feb 2021 05:57:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa219c983dff4f994e3a40eea7fe79b5cd8a401e095739cbcd515ef8513d078e`  
		Last Modified: Wed, 10 Feb 2021 05:58:43 GMT  
		Size: 3.8 MB (3804985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dd26452211bcf516ca9f4107f957017daa51834da7a18a386c53d71268f5dc`  
		Last Modified: Wed, 10 Feb 2021 05:59:11 GMT  
		Size: 87.1 MB (87128955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:554976c882252a014a151b7c06f499d7fd16fa867c461d4ad2da18a2feb55cf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110080393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f5f4c9d83020d090072c26ea47bdcdd3df372068f1e87d82d88d4e78c40ce6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:55:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 21:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:45:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c57aa437368cc78c67a8620d603f7b68778ebb227bd03a0a224d8fdf4aa488`  
		Last Modified: Tue, 09 Feb 2021 21:47:49 GMT  
		Size: 79.9 MB (79891106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:44cf61067e705e9f63790812f57a969d3e6dd8ad73e20c46aa93260ce78b34b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124860461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e74523be1d2ea57360b0af349ccbbfed50100c365f860c2fd920e325f413163`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:16:11 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 20:16:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bbec1829f62fe14d3a012d6c128c3ccf39cbe18cdc6ec5113c9ab8a6194dee`  
		Last Modified: Tue, 09 Feb 2021 20:19:49 GMT  
		Size: 92.5 MB (92498680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:511d712d1f83a691ce96eb4f6cabc89a6012024a0b6f73f4de5db048a2d24768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:a8cf8095c224b4149e40344a2c9b5ab7662dd2d5d28f892f62f3f7474faea8bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150421960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f75dc03bb02073b06ed205f78d93864e77d0c97cf0ab4b89ff7e96955f51ff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:37:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:37:36 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:37:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aff8b3c8cd719f99f940db3d69b9fdfd832dd1b472dab3cae6a3c5e0b6c291`  
		Last Modified: Tue, 09 Feb 2021 05:40:30 GMT  
		Size: 9.5 MB (9468394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0dc90c59f637f8c9d4f63c0a15bc869fe6405d52b19c37f47cf124f0c8c1da`  
		Last Modified: Tue, 09 Feb 2021 05:40:52 GMT  
		Size: 95.6 MB (95573681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:d8cef96661ca3b7a3f525ad90822c27b851fa5b889c2852aafe890224f619c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137443966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34499f98ea14274e201fee8cc738caab87934be61b8b2011e1b312b36a698bf`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 03:04:53 GMT
ADD file:f884b9fc23d1b8ad0bd21aa823afd0ee186bdebb6829ccba72f77caaeffd8d12 in / 
# Tue, 09 Feb 2021 03:04:55 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:17:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:17:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 03:17:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 03:17:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 03:17:18 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 05:58:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 Feb 2021 05:58:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5275c778c803ce7d82407c77cfad4fb07fd1ec80fc99ba94cef475a92e4d090c`  
		Last Modified: Tue, 09 Feb 2021 03:13:25 GMT  
		Size: 42.1 MB (42119892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33724ddfadc9df78f13b323674fdbf73e45f1d5096c0bce41f2d1fd9808019ff`  
		Last Modified: Wed, 10 Feb 2021 05:59:23 GMT  
		Size: 8.2 MB (8186473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea525324e712b7bdb3b2588fc9a27f73316246cee0c671d9a80ba668b64ce19`  
		Last Modified: Wed, 10 Feb 2021 05:59:47 GMT  
		Size: 87.1 MB (87137601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:81a289e1eeb92cfc09030a575ff664aa73b1bce223fab7a6a861e331079d33c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131523488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf9c3d4c205bd0fa72b56d6f58f8edae1293069d4818bb4040a7d1beee416aa`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:17 GMT
ADD file:fb69ff7b2a28f793efbd16e04b74ffb4557d39e1844b3789075b4d3ff97a0eaa in / 
# Tue, 09 Feb 2021 02:43:20 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:56:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:56:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:56:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:56:47 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 21:45:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:45:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:296c9f0bf5f2cf24e87bc5abd674fc486e8df419d4aa2d362453f64d38900504`  
		Last Modified: Tue, 09 Feb 2021 02:49:43 GMT  
		Size: 43.2 MB (43177550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65852c032a65dbd4a864997474741aff544a12e280cbd00b2b24755d862e19c7`  
		Last Modified: Tue, 09 Feb 2021 21:48:00 GMT  
		Size: 8.4 MB (8437015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e99d810313916e7e4e61ffa7ef5c000c1e6c6ddc2f115aa94fc4d55bdb2f58`  
		Last Modified: Tue, 09 Feb 2021 21:48:19 GMT  
		Size: 79.9 MB (79908923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:038fa0c0ce37234a69160e2841fe0938896f3a1f74879363feb5f94b96678dae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148073769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684ba79f7e666db1fe1dc39fa60c57933b0a83d7044c3202cc642e5dc8232e74`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:08 GMT
ADD file:4c25bc56152d0955bbdef26f612b172a90484913cbd1ab3332b3444c8c0c012e in / 
# Tue, 09 Feb 2021 02:42:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:17:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:17:04 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:17:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:17:05 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 09 Feb 2021 20:17:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:17:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5d7d8e56e51b8663a269c93107dcdf848d2f6a4f73ca51bb1ced208a1fa80c32`  
		Last Modified: Tue, 09 Feb 2021 02:49:23 GMT  
		Size: 46.1 MB (46097671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5fa89c1a6d759481e9dd18bf72ced3caf53e79be2ef6a132ac2a0115efb9b7`  
		Last Modified: Tue, 09 Feb 2021 20:19:57 GMT  
		Size: 9.5 MB (9474535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7a1c4781aa3b037108e1ec041dfbe9a58e7ae602497cb4696d0e9cddff0c47`  
		Last Modified: Tue, 09 Feb 2021 20:20:20 GMT  
		Size: 92.5 MB (92501563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:87795369570c665c79864d9b91ffda053404284522a00c670553ca9597722b8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.0-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:7cfd05f41e80511f98c789ab39eabbe40eb165cfc9f9048bdd2bbb69f126d090
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2546632000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4cbed689a02455eb3f26430cf502ff411c96e37869da13b0ea15f239a626b0`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:41:34 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:42:53 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:42:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c26da75e3692d075b8cc90f8e94e256478a20d09583dfb783167e2e0380194`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b98a5d75905f2eb4b3d70be1fe0d098358b64e50950c012cb9ecb05b3cfcecf`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451757b457dda2cb3a548462583261fb227d9adbca6abb5f1e2e952447e08431`  
		Last Modified: Wed, 10 Feb 2021 15:57:22 GMT  
		Size: 107.4 MB (107359734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa29bf77fc353bbde6f8398ea82e6863560e775323cdb11e6f8816ccb0055e9`  
		Last Modified: Wed, 10 Feb 2021 15:55:16 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:56c498b1c25d34165af969da8c0c0bf1a5ec739dbbc1f5b21e8992a296ff3972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:a043552752781077d5904fa96e3f394cb5d6e65f79e8b703e4af6188706e5c6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5903136908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66bfb21c71c4413d6a9ea1b509fec68b8ffe64d94698d3d8b7fd317dcbdd9eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:43:00 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 10 Feb 2021 15:43:01 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 10 Feb 2021 15:45:01 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:45:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf04a1bf70bc380723778f6b70ecc31a982c47090c0b72d56c1d534b6614c6`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54410ac5d0ad2c510f83f9d4cf7a5f393fd7e678ece07106faa2e90ff9473131`  
		Last Modified: Wed, 10 Feb 2021 15:57:35 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167063bef9cef158705c6ef5ae1f7576970568e6d06f95fd3fb89c45f5f9b654`  
		Last Modified: Wed, 10 Feb 2021 15:59:40 GMT  
		Size: 108.1 MB (108118430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeebbf24fc2c457e5491930a59cf8b87672aed1070138e3f42cc40d9520a199`  
		Last Modified: Wed, 10 Feb 2021 15:57:34 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5`

```console
$ docker pull julia@sha256:e7a4cb833d3078a68c4935e738d7b199c732ec0b120ce2c5fecc6e6d826bd318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.5` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3`

```console
$ docker pull julia@sha256:e7a4cb833d3078a68c4935e738d7b199c732ec0b120ce2c5fecc6e6d826bd318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.5.3` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-alpine`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5.3-alpine` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-alpine3.12`

```console
$ docker pull julia@sha256:690aa7c9f1c3ba60a239c7fbe4fc902b2c6d0706a87b6ceaf39acfe22463ae7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5.3-alpine3.12` - linux; amd64

```console
$ docker pull julia@sha256:468f0c82b4e051d1ceb9990f1218d381b85d8f9494cd8a0ea3133396594e163d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112509391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb5e38938cfb1e5a635d3be992f69564d5c693ce9b93055a5c20967f058920e`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:05:39 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 17 Dec 2020 13:05:39 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_VERSION=1.5.3
# Thu, 17 Dec 2020 13:05:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 17 Dec 2020 13:05:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4826849b1ea579b0d13b4f603ea4aa1187d74764b579dc0cd40ad66e51049adc`  
		Last Modified: Thu, 17 Dec 2020 13:07:07 GMT  
		Size: 109.7 MB (109710325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-alpine3.13`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5.3-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-buster`

```console
$ docker pull julia@sha256:64fd28a8a228d414164da6ad71cb9ac4495a5dafa05d58711271016b2ff718f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.5.3-buster` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3-buster` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-windowsservercore-1809`

```console
$ docker pull julia@sha256:bff8e8031e0163ba103115157191ae4f06cf50fd9e9cc79779804bab7207ed2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.5.3-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:26302de5bf7ef96403110882de21a7997fd16bb2b79e6c90114c31f99c1bbb97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.5.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-alpine`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5-alpine` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-alpine3.12`

```console
$ docker pull julia@sha256:690aa7c9f1c3ba60a239c7fbe4fc902b2c6d0706a87b6ceaf39acfe22463ae7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5-alpine3.12` - linux; amd64

```console
$ docker pull julia@sha256:468f0c82b4e051d1ceb9990f1218d381b85d8f9494cd8a0ea3133396594e163d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112509391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb5e38938cfb1e5a635d3be992f69564d5c693ce9b93055a5c20967f058920e`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:05:39 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 17 Dec 2020 13:05:39 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_VERSION=1.5.3
# Thu, 17 Dec 2020 13:05:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 17 Dec 2020 13:05:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4826849b1ea579b0d13b4f603ea4aa1187d74764b579dc0cd40ad66e51049adc`  
		Last Modified: Thu, 17 Dec 2020 13:07:07 GMT  
		Size: 109.7 MB (109710325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-alpine3.13`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-buster`

```console
$ docker pull julia@sha256:64fd28a8a228d414164da6ad71cb9ac4495a5dafa05d58711271016b2ff718f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5-buster` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:bff8e8031e0163ba103115157191ae4f06cf50fd9e9cc79779804bab7207ed2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.5-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:26302de5bf7ef96403110882de21a7997fd16bb2b79e6c90114c31f99c1bbb97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:95b7c7ec415ce07fd49f733d4a3e04faf6535d0552f9ed99d212ecc466ee4020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0`

```console
$ docker pull julia@sha256:95b7c7ec415ce07fd49f733d4a3e04faf6535d0552f9ed99d212ecc466ee4020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6.0` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-buster`

```console
$ docker pull julia@sha256:a68683d3e50fea0ca19095259deea0f15760537c4740ffd8be23073a66f15e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-buster` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-rc1`

```console
$ docker pull julia@sha256:95b7c7ec415ce07fd49f733d4a3e04faf6535d0552f9ed99d212ecc466ee4020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6.0-rc1` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-rc1-buster`

```console
$ docker pull julia@sha256:a68683d3e50fea0ca19095259deea0f15760537c4740ffd8be23073a66f15e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6.0-rc1-buster` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1-buster` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-rc1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-rc1-windowsservercore-1809`

```console
$ docker pull julia@sha256:5855f20ad40c971e35e38632a0766cc7bd787d9e159e09c665656048890e3874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.6.0-rc1-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-rc1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:db937302e1505024ea82c09f2171f1695fa9a3fb11fd3db311b7fc2127697394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6.0-rc1-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:5855f20ad40c971e35e38632a0766cc7bd787d9e159e09c665656048890e3874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.6.0-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:db937302e1505024ea82c09f2171f1695fa9a3fb11fd3db311b7fc2127697394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:a68683d3e50fea0ca19095259deea0f15760537c4740ffd8be23073a66f15e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc`

```console
$ docker pull julia@sha256:95b7c7ec415ce07fd49f733d4a3e04faf6535d0552f9ed99d212ecc466ee4020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6-rc` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc-buster`

```console
$ docker pull julia@sha256:a68683d3e50fea0ca19095259deea0f15760537c4740ffd8be23073a66f15e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6-rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:644f53101686e8d272784813b145bde90b476b2f257ca4d59ada41227685972c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152640649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8535db39a656e88b5219f82b7e1f4b3f2c9da053ea78888f89374017c5700b10`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 05:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e02d4ebb1f940ce66315d1d9ffe72a654f2eaf894d4a215558f0f61b2b6d7f9`  
		Last Modified: Tue, 09 Feb 2021 05:39:02 GMT  
		Size: 121.1 MB (121089569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ad782626b772257845b8c044b20e3cb6e95e978181380e3a743cc8c5569d1a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145118295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb17c7662e1342def5ac7e0719d5acfdbdf282db97b566618dc29596f7506ae`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:53:23 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 21:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:43:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb3a915708fc1e20ff2e66ab9a51a3a1ced003c56c32de6e2e8f27412d270b`  
		Last Modified: Tue, 09 Feb 2021 21:46:38 GMT  
		Size: 114.9 MB (114929008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc-buster` - linux; 386

```console
$ docker pull julia@sha256:c73ed17cb3c4bfb71338807a452e47d10c9d6e37284bb003777274afb4e513d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151234207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe4159eff98ef296a316ff1065aa9bbbe9a43062f8bc3bd83a32fd7cfd00aac`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 20:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e588627db6401a1c5f85f6aa3732e452b91729b96288d6a7b152d17ddb3ba`  
		Last Modified: Tue, 09 Feb 2021 20:18:39 GMT  
		Size: 118.9 MB (118872426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:ae2380d0ec5fc9ebc9ffba0bc4edc57d702d2bc5e89880a1555206e3caba2414
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a3f4e19008592a819da8d32f2aa4b43f5c66cb3c8c4ab43399ca2702fb80da`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:41:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 09:41:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 09:41:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 09:42:00 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Tue, 09 Feb 2021 09:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='72847bd2b4d4db9d5970512f79fd5a7f76ad56cf0f2ea5a80eff032364b19c8b' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='4f11cad2b0e2d64980b1cb66a327ed19d9ffadabedb6391ea901ccdc45f983b5' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='bf131902325559594da0a77f23d58a3161b4280f9d3b7c970614bf1b258431c4' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='1e6c7960394d60bbef4f5813db421b7dbfce8bdcc9218657d52256cb56e9fad6' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 09:43:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbde24ad7b5b0c5354eb358ac5242efd49b308f924d96cc9bab94697d0c07a5`  
		Last Modified: Tue, 09 Feb 2021 09:44:25 GMT  
		Size: 4.9 MB (4853658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1cf1e7ac5be9e529a67bc676f930f253081bce226627aa5ae5e1bd7817fe66`  
		Last Modified: Tue, 09 Feb 2021 09:44:46 GMT  
		Size: 106.4 MB (106433976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:5855f20ad40c971e35e38632a0766cc7bd787d9e159e09c665656048890e3874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.6-rc-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:db937302e1505024ea82c09f2171f1695fa9a3fb11fd3db311b7fc2127697394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6-rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:5855f20ad40c971e35e38632a0766cc7bd787d9e159e09c665656048890e3874
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:da731ca937b864fe0f540699c8eff3f7b09609df0e751d5b7c6161bb34b568be
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581448539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efda81923536ba00e65e3e35a782121af9ebc2b2c4127279c57d7a87d902edb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:33:33 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:33:34 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:35:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:35:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375559cf73cb5a1f3ec1a3c422e5bcbda269f2ff82cf10f55052cdc26ae4b0f2`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ce66d0c0671c836605f71620b9d7c9ca3ed5c7afe19b1e2d354b7fc66ccfd`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20c879fe6e4f0cc4b668ffa9053de0695e60ed57f483d3dff4425c76c1cf3b`  
		Last Modified: Wed, 10 Feb 2021 15:48:27 GMT  
		Size: 142.2 MB (142176319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9b38c90003053d015f9a0ec6d10918553864d71f25bd5008a6bb964b791d09`  
		Last Modified: Wed, 10 Feb 2021 15:45:49 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:db937302e1505024ea82c09f2171f1695fa9a3fb11fd3db311b7fc2127697394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:b3a41195710bce40099556982198922ac65c48563f6d9be9c212b5eaa0e456f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937962882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35d4978b7f7beced87907c4d6af4c7417c94d504e8cde40a3ea19ef9c341e27`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_VERSION=1.6.0-rc1
# Wed, 10 Feb 2021 15:35:15 GMT
ENV JULIA_SHA256=7a81fa6d83d2e15b38b794006d2bf4731134c530113584d3b40497209d100bd4
# Wed, 10 Feb 2021 15:37:27 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:37:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2db5beb759bbb97a8f3da7251caf6f0ef6192f1515eaaaf283ac91536dde`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a4f1366db8a4a3adbea683b7d564c8ac03e3bffa62ff339b33885e6f1055b`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d887bdd70a1d82147a03a333cc1f449d0218b4b99eb5bd5466418c35d23add0`  
		Last Modified: Wed, 10 Feb 2021 15:51:18 GMT  
		Size: 142.9 MB (142944498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fae921797af17e691d77fd53c75c70d70e4dd77570385de64f4d932363a542`  
		Last Modified: Wed, 10 Feb 2021 15:48:43 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.12`

```console
$ docker pull julia@sha256:690aa7c9f1c3ba60a239c7fbe4fc902b2c6d0706a87b6ceaf39acfe22463ae7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine3.12` - linux; amd64

```console
$ docker pull julia@sha256:468f0c82b4e051d1ceb9990f1218d381b85d8f9494cd8a0ea3133396594e163d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112509391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb5e38938cfb1e5a635d3be992f69564d5c693ce9b93055a5c20967f058920e`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:05:39 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 17 Dec 2020 13:05:39 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_VERSION=1.5.3
# Thu, 17 Dec 2020 13:05:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 17 Dec 2020 13:05:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4826849b1ea579b0d13b4f603ea4aa1187d74764b579dc0cd40ad66e51049adc`  
		Last Modified: Thu, 17 Dec 2020 13:07:07 GMT  
		Size: 109.7 MB (109710325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.13`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:64fd28a8a228d414164da6ad71cb9ac4495a5dafa05d58711271016b2ff718f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:bff8e8031e0163ba103115157191ae4f06cf50fd9e9cc79779804bab7207ed2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:26302de5bf7ef96403110882de21a7997fd16bb2b79e6c90114c31f99c1bbb97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.12`

```console
$ docker pull julia@sha256:690aa7c9f1c3ba60a239c7fbe4fc902b2c6d0706a87b6ceaf39acfe22463ae7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine3.12` - linux; amd64

```console
$ docker pull julia@sha256:468f0c82b4e051d1ceb9990f1218d381b85d8f9494cd8a0ea3133396594e163d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112509391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb5e38938cfb1e5a635d3be992f69564d5c693ce9b93055a5c20967f058920e`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:05:39 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 17 Dec 2020 13:05:39 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 17 Dec 2020 13:05:40 GMT
ENV JULIA_VERSION=1.5.3
# Thu, 17 Dec 2020 13:05:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 17 Dec 2020 13:05:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4826849b1ea579b0d13b4f603ea4aa1187d74764b579dc0cd40ad66e51049adc`  
		Last Modified: Thu, 17 Dec 2020 13:07:07 GMT  
		Size: 109.7 MB (109710325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.13`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:64fd28a8a228d414164da6ad71cb9ac4495a5dafa05d58711271016b2ff718f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:e7a4cb833d3078a68c4935e738d7b199c732ec0b120ce2c5fecc6e6d826bd318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:d55accec94b302a610f2edcec3312a5d858e5ccb7be3362c7d666530664abdfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144611151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0796d56b70aa43f2a18076fe4527ac6b3851aabc85cb5d04f17841340a6829`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:35:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 05:35:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 05:35:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 05:36:22 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 05:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 05:36:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2772078caadc07d8e4898c46d6e77ed570b46a2852bfe578ee085bfc4c937`  
		Last Modified: Tue, 09 Feb 2021 05:38:33 GMT  
		Size: 4.5 MB (4455938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879eb1e914debfd7ed46f3f0708f8aeaca2b4ba7255a8ec30c446ccb0d89d3e2`  
		Last Modified: Tue, 09 Feb 2021 05:39:44 GMT  
		Size: 113.1 MB (113060071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b1f99a248e3dc3ac40b13c32e2b6919ed102ba6a0c9f60f06208d4a7739828d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135561113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b9594902102907ac815c9157ef7eec27a1a7509e040e748a2b5717ac60244c`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 02:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 02:53:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 02:53:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 02:54:17 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 21:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 21:44:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33af1c26fb4ce81cf943a709652891fb909f64b1b467b517cb5557be13a222`  
		Last Modified: Tue, 09 Feb 2021 21:46:10 GMT  
		Size: 4.3 MB (4337838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29088ea75a6fc6fc34b9fc490e00f62f5231dde0a22d29b15b1693a34c1a71f`  
		Last Modified: Tue, 09 Feb 2021 21:47:17 GMT  
		Size: 105.4 MB (105371826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:cbd1cad24e60efe33ec0cdae3c8428ba9f242f58234f987a26949d97b30bb2a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142431421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108deea0c7d0b3f7baef3deca6b6b5f4d3ffdb49f813ca750f0fdae11828133b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 20:14:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:14:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Feb 2021 20:14:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:14:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Feb 2021 20:15:29 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 09 Feb 2021 20:16:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 09 Feb 2021 20:16:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9db8529c8fa440f206e4f00b1cff5513459ce2d7e8f74c3797796c275a2067`  
		Last Modified: Tue, 09 Feb 2021 20:18:06 GMT  
		Size: 4.6 MB (4609050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9d2c08b6fd1937f7dd03818dad58b493a0ce893129cce192ea99ba8210397`  
		Last Modified: Tue, 09 Feb 2021 20:19:16 GMT  
		Size: 110.1 MB (110069640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:bff8e8031e0163ba103115157191ae4f06cf50fd9e9cc79779804bab7207ed2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull julia@sha256:34f3b5b4f2b7abb4a1bec3d709154d0f7c57707e4b1784f6044a92d8412b1cf1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576317627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8f9536c5bf1012f5dbe1f04344701b94a3d7112c99163e4b8763db1c3d226`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:37:41 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:39:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:39:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a770b09ae561ef072f35bc39e3a11ba203b0de0cb99229d5ea041b8c02ada7`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21fc225c30062be01308131b711cf4354b7264c5033a0436e87ce8d9c2d088`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f96679f3443215bd1c7cdfd04ccde2ca3a4a5efcc204880658717533141da2`  
		Last Modified: Wed, 10 Feb 2021 15:52:04 GMT  
		Size: 137.0 MB (137045356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf7d11dcb516965af0d0c2450a64b68287c6f7d0167fc34f497f3c2ce05335f`  
		Last Modified: Wed, 10 Feb 2021 15:51:35 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:26302de5bf7ef96403110882de21a7997fd16bb2b79e6c90114c31f99c1bbb97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull julia@sha256:2fbc17fd3df3611b2942477a521b8192c5984374eab729ea1ac5057a4ab388f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5932839062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a36a7004d1a5915e7c70a6c62e418e33f8527b5d07098fdac0c825de341457`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 10 Feb 2021 15:39:22 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 10 Feb 2021 15:41:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 15:41:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7042a225a09bd32d6b88acda4b3fd9d5d905bf5c152fd569196f68c1840e2`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f9db5fe8cd82480573b32904348be5e98daac412b173f4d3365249516154b7`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf021c7aeb47f1feb924581337b72b863cdea144956492a668c8691eb697a6`  
		Last Modified: Wed, 10 Feb 2021 15:54:59 GMT  
		Size: 137.8 MB (137820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d39424c2ac2d83ea22a565e4485bd34b567392a8d3a1df7cf73fa93de3f8a`  
		Last Modified: Wed, 10 Feb 2021 15:52:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
