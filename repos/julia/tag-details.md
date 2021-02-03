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
-	[`julia:1.6.0-beta1`](#julia160-beta1)
-	[`julia:1.6.0-beta1-buster`](#julia160-beta1-buster)
-	[`julia:1.6.0-beta1-windowsservercore-1809`](#julia160-beta1-windowsservercore-1809)
-	[`julia:1.6.0-beta1-windowsservercore-ltsc2016`](#julia160-beta1-windowsservercore-ltsc2016)
-	[`julia:1.6.0-buster`](#julia160-buster)
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
$ docker pull julia@sha256:1a1bb9b9d33e5df42f9d50aaaf9775d955bc49a24404ef54a0fa48875111732c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:b8f8a8977329ceaa266c705b16a828b5b842dfdd9f513d5d0fe36c9488367916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:d67eafef84df1c702cbb58051e21a5a31345adecb5c3bf00c671f29a21b56051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127108211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa712fbd4643c27265cd03f037c67800452ec4af44253c3897833c53a5c9cebe`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:33:09 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 09:33:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:33:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e616ad53f43c235db61a2fd232ebc2621bfdbfd40dfd922d865b1a66069cbc`  
		Last Modified: Tue, 12 Jan 2021 09:37:02 GMT  
		Size: 95.6 MB (95563187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:da9a4942d89023c20641b805931515d938c30423317821e7acc461630fb40edc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113619490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13843a9f82e57a93ec771dfe82e8b700dc0b499c2769d75e8e4772830049e7e2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:00:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:00:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:00:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:00:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:00:14 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:01:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:01:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6a485ade5fe8251540ff32a0c7b2421132d4d12d0d9ad19f199462b5362346`  
		Last Modified: Fri, 11 Dec 2020 16:03:10 GMT  
		Size: 3.8 MB (3782951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb73228fce12bc424cd539af15455353df573822b4215e70cc6adea7c29109`  
		Last Modified: Fri, 11 Dec 2020 16:03:40 GMT  
		Size: 87.1 MB (87128877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a47cc607820cda2c990c087405c5655c285b23e66726fa2ef71851334aabfdeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110062389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22e8964174b44a1fd2b2dd2dcffd9e99bacab2e841939cef24822c619808e74`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:47:29 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:47:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54699d638f2f6414aae4721f51101f031299ec3bbc38dcaf708f8d2a584156a2`  
		Last Modified: Fri, 11 Dec 2020 16:50:42 GMT  
		Size: 79.9 MB (79891001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:9262d8151c955d959ce8a6d4af4580725dbaa7b024d557b4f700df87fee2fbb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124852914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d2d03e545fd69f5d38211554f38472e3fcec7edd3d8733641f7f6fc03dfdb7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:45:29 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 03:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65befa293aa08004e1c19d2e998fc1d57ab7d19859bde2149191dcf78b3a8cc`  
		Last Modified: Tue, 12 Jan 2021 03:48:54 GMT  
		Size: 92.5 MB (92498553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:fdb8539819660ff503bd662be2901cdce1b03fe1141c92883a60e05d46f58545
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2543079070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64888b637748e8242b8e2aacf412a234514184b731a8f2f54ea067b1563cd1ce`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:51:57 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:51:58 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:54:07 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:54:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d455d90e93f5eada528324775225d40a7a1550c6592b94e0ca492edbb3eecbd`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539e4779ae807fba7ee5490c9de973bcc5a2732e5cc8b7f151b95238051d9b9`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144a18fadb6c2512ef580ea9d52e5fb41995c189c297843fd2b58b66eee71dab`  
		Last Modified: Wed, 13 Jan 2021 19:02:24 GMT  
		Size: 107.3 MB (107302414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3bd53ab29546094935034aa7b475c582b0a5e7ebe1ad866ef2de8194745952`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:54139b747e8989c5b9dd1b782cedd068db26df94dffa3cd01a93fc10f510013c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5901999287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5700a05b11510e95fe0f03623b20428d2d71cf2b5b08735d2b66e1eefdb10e48`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:54:23 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:54:24 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:57:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:57:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a5352a2cb4c292314199884a957537c41ff1d8129b9b1b6ee38e5371cd7878`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb57a5b62ded9f8545dcc267b92de5d3ce66ab3b2faff3ee1149c238a66ae6`  
		Last Modified: Wed, 13 Jan 2021 19:02:42 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928d7681603fff97b6322d1e7e4fc7b114e4b5030782dfc407f159fa468cf3f6`  
		Last Modified: Wed, 13 Jan 2021 19:03:04 GMT  
		Size: 108.1 MB (108100699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a97fd0203f542a9ba2737df2071b68283aa7fbcb59e222a94f1eadffba4f5`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:b8f8a8977329ceaa266c705b16a828b5b842dfdd9f513d5d0fe36c9488367916
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:d67eafef84df1c702cbb58051e21a5a31345adecb5c3bf00c671f29a21b56051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127108211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa712fbd4643c27265cd03f037c67800452ec4af44253c3897833c53a5c9cebe`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:33:09 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 09:33:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:33:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e616ad53f43c235db61a2fd232ebc2621bfdbfd40dfd922d865b1a66069cbc`  
		Last Modified: Tue, 12 Jan 2021 09:37:02 GMT  
		Size: 95.6 MB (95563187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:da9a4942d89023c20641b805931515d938c30423317821e7acc461630fb40edc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113619490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13843a9f82e57a93ec771dfe82e8b700dc0b499c2769d75e8e4772830049e7e2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:00:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:00:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:00:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:00:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:00:14 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:01:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:01:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6a485ade5fe8251540ff32a0c7b2421132d4d12d0d9ad19f199462b5362346`  
		Last Modified: Fri, 11 Dec 2020 16:03:10 GMT  
		Size: 3.8 MB (3782951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb73228fce12bc424cd539af15455353df573822b4215e70cc6adea7c29109`  
		Last Modified: Fri, 11 Dec 2020 16:03:40 GMT  
		Size: 87.1 MB (87128877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a47cc607820cda2c990c087405c5655c285b23e66726fa2ef71851334aabfdeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110062389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22e8964174b44a1fd2b2dd2dcffd9e99bacab2e841939cef24822c619808e74`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:47:29 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:47:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54699d638f2f6414aae4721f51101f031299ec3bbc38dcaf708f8d2a584156a2`  
		Last Modified: Fri, 11 Dec 2020 16:50:42 GMT  
		Size: 79.9 MB (79891001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:9262d8151c955d959ce8a6d4af4580725dbaa7b024d557b4f700df87fee2fbb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124852914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d2d03e545fd69f5d38211554f38472e3fcec7edd3d8733641f7f6fc03dfdb7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:45:29 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 03:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65befa293aa08004e1c19d2e998fc1d57ab7d19859bde2149191dcf78b3a8cc`  
		Last Modified: Tue, 12 Jan 2021 03:48:54 GMT  
		Size: 92.5 MB (92498553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:fdb8539819660ff503bd662be2901cdce1b03fe1141c92883a60e05d46f58545
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2543079070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64888b637748e8242b8e2aacf412a234514184b731a8f2f54ea067b1563cd1ce`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:51:57 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:51:58 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:54:07 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:54:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d455d90e93f5eada528324775225d40a7a1550c6592b94e0ca492edbb3eecbd`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539e4779ae807fba7ee5490c9de973bcc5a2732e5cc8b7f151b95238051d9b9`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144a18fadb6c2512ef580ea9d52e5fb41995c189c297843fd2b58b66eee71dab`  
		Last Modified: Wed, 13 Jan 2021 19:02:24 GMT  
		Size: 107.3 MB (107302414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3bd53ab29546094935034aa7b475c582b0a5e7ebe1ad866ef2de8194745952`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:54139b747e8989c5b9dd1b782cedd068db26df94dffa3cd01a93fc10f510013c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5901999287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5700a05b11510e95fe0f03623b20428d2d71cf2b5b08735d2b66e1eefdb10e48`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:54:23 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:54:24 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:57:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:57:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a5352a2cb4c292314199884a957537c41ff1d8129b9b1b6ee38e5371cd7878`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb57a5b62ded9f8545dcc267b92de5d3ce66ab3b2faff3ee1149c238a66ae6`  
		Last Modified: Wed, 13 Jan 2021 19:02:42 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928d7681603fff97b6322d1e7e4fc7b114e4b5030782dfc407f159fa468cf3f6`  
		Last Modified: Wed, 13 Jan 2021 19:03:04 GMT  
		Size: 108.1 MB (108100699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a97fd0203f542a9ba2737df2071b68283aa7fbcb59e222a94f1eadffba4f5`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:283d15baed6f4f1239d05f75b30e3062cae0f2521151caf38d7df62eaa3afd76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:d67eafef84df1c702cbb58051e21a5a31345adecb5c3bf00c671f29a21b56051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127108211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa712fbd4643c27265cd03f037c67800452ec4af44253c3897833c53a5c9cebe`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:33:09 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 09:33:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:33:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e616ad53f43c235db61a2fd232ebc2621bfdbfd40dfd922d865b1a66069cbc`  
		Last Modified: Tue, 12 Jan 2021 09:37:02 GMT  
		Size: 95.6 MB (95563187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:da9a4942d89023c20641b805931515d938c30423317821e7acc461630fb40edc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113619490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13843a9f82e57a93ec771dfe82e8b700dc0b499c2769d75e8e4772830049e7e2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:00:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:00:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:00:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:00:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:00:14 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:01:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:01:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6a485ade5fe8251540ff32a0c7b2421132d4d12d0d9ad19f199462b5362346`  
		Last Modified: Fri, 11 Dec 2020 16:03:10 GMT  
		Size: 3.8 MB (3782951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb73228fce12bc424cd539af15455353df573822b4215e70cc6adea7c29109`  
		Last Modified: Fri, 11 Dec 2020 16:03:40 GMT  
		Size: 87.1 MB (87128877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a47cc607820cda2c990c087405c5655c285b23e66726fa2ef71851334aabfdeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110062389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22e8964174b44a1fd2b2dd2dcffd9e99bacab2e841939cef24822c619808e74`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:47:29 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:47:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54699d638f2f6414aae4721f51101f031299ec3bbc38dcaf708f8d2a584156a2`  
		Last Modified: Fri, 11 Dec 2020 16:50:42 GMT  
		Size: 79.9 MB (79891001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:9262d8151c955d959ce8a6d4af4580725dbaa7b024d557b4f700df87fee2fbb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124852914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d2d03e545fd69f5d38211554f38472e3fcec7edd3d8733641f7f6fc03dfdb7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:45:29 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 03:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65befa293aa08004e1c19d2e998fc1d57ab7d19859bde2149191dcf78b3a8cc`  
		Last Modified: Tue, 12 Jan 2021 03:48:54 GMT  
		Size: 92.5 MB (92498553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:86694ddc4fc05d5aaa7ad1a5b11b0a3d7dd3b22392b9512cf5b7b9020809fd25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:f40185ed4b71cfd3014c6c78675197093e25c89065769e84dba95b6c2fdf134f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150421661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c45ec4f7b5a8f7e9b929a8432e3207c763a38c38530af93386640bc6d18853eb`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:33:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:33:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:33:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:33:52 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 09:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:34:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757033fa7836fe18ccac7ad43b92f69eb6bcfde0161200c35e9dfb75d20a000f`  
		Last Modified: Tue, 12 Jan 2021 09:37:18 GMT  
		Size: 9.5 MB (9467970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa3c8618d08c4c999315443e3a4c0ee137e4c83501f4fe72a9fb36e489ca7a`  
		Last Modified: Tue, 12 Jan 2021 09:37:43 GMT  
		Size: 95.6 MB (95573677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:ebdd432cbf99891dd447a54a602e0971a157966e6e838340b1de6193d88bbaef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137440122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5787c9c76872eb4c56562c6acff6bef0b5492533fa225b4bb42935d611685bda`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:02:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:02:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:02:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:02:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:02:20 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:02:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:02:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffba9fe2a24169edb23d38e80ced3ee939e2c706ef1ad723e882e50ab2f2aa2c`  
		Last Modified: Fri, 11 Dec 2020 16:03:51 GMT  
		Size: 8.2 MB (8184526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b5cc0459eea712568373d8be5500a14ecf3da4528325b2a10d7341c4510c99`  
		Last Modified: Fri, 11 Dec 2020 16:04:18 GMT  
		Size: 87.1 MB (87137647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c2f240cd6b56f1bcb4e6085af752513d2ec31c9434ca271ddcf31583207811e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131520467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8532042852f37450bcb38277a275f71ca0f5d9ffb0e61bb9f77b740bfc16eabf`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:48:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:48:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:48:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:48:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:48:45 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:49:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:49:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7717de1dafcd768ea7bc31f1c27312ccc907fa240bc062dacf26ae847487d9b6`  
		Last Modified: Fri, 11 Dec 2020 16:51:01 GMT  
		Size: 8.4 MB (8435533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc321b05ebfe4d813df8172175b53fe7c7d781fa1270dae4db009b5b3ac7dbea`  
		Last Modified: Fri, 11 Dec 2020 16:51:12 GMT  
		Size: 79.9 MB (79908993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:f47fec8d06ebc800ea04b33534adad40a8e413e11e1b84436b8d693c7a0b0d66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148073341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c05250fc229ef58d38c48c6b1e0f02d35dfc6421f8c34a5ab493c0f827c3282`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:00 GMT
ADD file:0da7fb4b520f7df6963291eabeab1e021ecc9f8fa5507ea307b64cd109898702 in / 
# Tue, 12 Jan 2021 00:42:00 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:46:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:46:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:46:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:46:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:46:09 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 03:46:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:46:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9200bc3dda820226401b71a8464b0ea725d889387e461c9cf3d8155012f09f94`  
		Last Modified: Tue, 12 Jan 2021 00:50:31 GMT  
		Size: 46.1 MB (46097646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982baf29c259b18c146a22e25278539fc7e5f9cc0b6e2158a567c0922df487ce`  
		Last Modified: Tue, 12 Jan 2021 03:49:05 GMT  
		Size: 9.5 MB (9474125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc9c9a7b851c579ac8dac027ca82c6ee83b0f0c7e950503d59bd350badbe6c`  
		Last Modified: Tue, 12 Jan 2021 03:49:27 GMT  
		Size: 92.5 MB (92501570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:ea4f8715711afb573a6e3c2613975886ac7aed3d3f7c6681ee461a493bfcb1bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.0.5-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:fdb8539819660ff503bd662be2901cdce1b03fe1141c92883a60e05d46f58545
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2543079070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64888b637748e8242b8e2aacf412a234514184b731a8f2f54ea067b1563cd1ce`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:51:57 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:51:58 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:54:07 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:54:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d455d90e93f5eada528324775225d40a7a1550c6592b94e0ca492edbb3eecbd`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539e4779ae807fba7ee5490c9de973bcc5a2732e5cc8b7f151b95238051d9b9`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144a18fadb6c2512ef580ea9d52e5fb41995c189c297843fd2b58b66eee71dab`  
		Last Modified: Wed, 13 Jan 2021 19:02:24 GMT  
		Size: 107.3 MB (107302414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3bd53ab29546094935034aa7b475c582b0a5e7ebe1ad866ef2de8194745952`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:4a147398f6f0e446f55a11aa0320c92e61fdb026e2cfe37c8eb966005e6e1888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:54139b747e8989c5b9dd1b782cedd068db26df94dffa3cd01a93fc10f510013c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5901999287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5700a05b11510e95fe0f03623b20428d2d71cf2b5b08735d2b66e1eefdb10e48`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:54:23 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:54:24 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:57:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:57:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a5352a2cb4c292314199884a957537c41ff1d8129b9b1b6ee38e5371cd7878`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb57a5b62ded9f8545dcc267b92de5d3ce66ab3b2faff3ee1149c238a66ae6`  
		Last Modified: Wed, 13 Jan 2021 19:02:42 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928d7681603fff97b6322d1e7e4fc7b114e4b5030782dfc407f159fa468cf3f6`  
		Last Modified: Wed, 13 Jan 2021 19:03:04 GMT  
		Size: 108.1 MB (108100699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a97fd0203f542a9ba2737df2071b68283aa7fbcb59e222a94f1eadffba4f5`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:283d15baed6f4f1239d05f75b30e3062cae0f2521151caf38d7df62eaa3afd76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:d67eafef84df1c702cbb58051e21a5a31345adecb5c3bf00c671f29a21b56051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127108211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa712fbd4643c27265cd03f037c67800452ec4af44253c3897833c53a5c9cebe`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:33:09 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 09:33:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:33:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e616ad53f43c235db61a2fd232ebc2621bfdbfd40dfd922d865b1a66069cbc`  
		Last Modified: Tue, 12 Jan 2021 09:37:02 GMT  
		Size: 95.6 MB (95563187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:da9a4942d89023c20641b805931515d938c30423317821e7acc461630fb40edc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113619490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13843a9f82e57a93ec771dfe82e8b700dc0b499c2769d75e8e4772830049e7e2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:00:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:00:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:00:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:00:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:00:14 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:01:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:01:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6a485ade5fe8251540ff32a0c7b2421132d4d12d0d9ad19f199462b5362346`  
		Last Modified: Fri, 11 Dec 2020 16:03:10 GMT  
		Size: 3.8 MB (3782951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb73228fce12bc424cd539af15455353df573822b4215e70cc6adea7c29109`  
		Last Modified: Fri, 11 Dec 2020 16:03:40 GMT  
		Size: 87.1 MB (87128877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a47cc607820cda2c990c087405c5655c285b23e66726fa2ef71851334aabfdeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110062389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22e8964174b44a1fd2b2dd2dcffd9e99bacab2e841939cef24822c619808e74`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:47:29 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:47:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54699d638f2f6414aae4721f51101f031299ec3bbc38dcaf708f8d2a584156a2`  
		Last Modified: Fri, 11 Dec 2020 16:50:42 GMT  
		Size: 79.9 MB (79891001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:9262d8151c955d959ce8a6d4af4580725dbaa7b024d557b4f700df87fee2fbb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124852914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d2d03e545fd69f5d38211554f38472e3fcec7edd3d8733641f7f6fc03dfdb7`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:45:29 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 03:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65befa293aa08004e1c19d2e998fc1d57ab7d19859bde2149191dcf78b3a8cc`  
		Last Modified: Tue, 12 Jan 2021 03:48:54 GMT  
		Size: 92.5 MB (92498553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:86694ddc4fc05d5aaa7ad1a5b11b0a3d7dd3b22392b9512cf5b7b9020809fd25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:f40185ed4b71cfd3014c6c78675197093e25c89065769e84dba95b6c2fdf134f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150421661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c45ec4f7b5a8f7e9b929a8432e3207c763a38c38530af93386640bc6d18853eb`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:33:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:33:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:33:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:33:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:33:52 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 09:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:34:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757033fa7836fe18ccac7ad43b92f69eb6bcfde0161200c35e9dfb75d20a000f`  
		Last Modified: Tue, 12 Jan 2021 09:37:18 GMT  
		Size: 9.5 MB (9467970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa3c8618d08c4c999315443e3a4c0ee137e4c83501f4fe72a9fb36e489ca7a`  
		Last Modified: Tue, 12 Jan 2021 09:37:43 GMT  
		Size: 95.6 MB (95573677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:ebdd432cbf99891dd447a54a602e0971a157966e6e838340b1de6193d88bbaef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137440122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5787c9c76872eb4c56562c6acff6bef0b5492533fa225b4bb42935d611685bda`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:02:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:02:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:02:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:02:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:02:20 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:02:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:02:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffba9fe2a24169edb23d38e80ced3ee939e2c706ef1ad723e882e50ab2f2aa2c`  
		Last Modified: Fri, 11 Dec 2020 16:03:51 GMT  
		Size: 8.2 MB (8184526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b5cc0459eea712568373d8be5500a14ecf3da4528325b2a10d7341c4510c99`  
		Last Modified: Fri, 11 Dec 2020 16:04:18 GMT  
		Size: 87.1 MB (87137647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c2f240cd6b56f1bcb4e6085af752513d2ec31c9434ca271ddcf31583207811e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131520467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8532042852f37450bcb38277a275f71ca0f5d9ffb0e61bb9f77b740bfc16eabf`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:48:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:48:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:48:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:48:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:48:45 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 11 Dec 2020 16:49:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:49:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7717de1dafcd768ea7bc31f1c27312ccc907fa240bc062dacf26ae847487d9b6`  
		Last Modified: Fri, 11 Dec 2020 16:51:01 GMT  
		Size: 8.4 MB (8435533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc321b05ebfe4d813df8172175b53fe7c7d781fa1270dae4db009b5b3ac7dbea`  
		Last Modified: Fri, 11 Dec 2020 16:51:12 GMT  
		Size: 79.9 MB (79908993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:f47fec8d06ebc800ea04b33534adad40a8e413e11e1b84436b8d693c7a0b0d66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148073341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c05250fc229ef58d38c48c6b1e0f02d35dfc6421f8c34a5ab493c0f827c3282`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:00 GMT
ADD file:0da7fb4b520f7df6963291eabeab1e021ecc9f8fa5507ea307b64cd109898702 in / 
# Tue, 12 Jan 2021 00:42:00 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:46:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:46:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:46:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:46:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:46:09 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 12 Jan 2021 03:46:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:46:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9200bc3dda820226401b71a8464b0ea725d889387e461c9cf3d8155012f09f94`  
		Last Modified: Tue, 12 Jan 2021 00:50:31 GMT  
		Size: 46.1 MB (46097646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982baf29c259b18c146a22e25278539fc7e5f9cc0b6e2158a567c0922df487ce`  
		Last Modified: Tue, 12 Jan 2021 03:49:05 GMT  
		Size: 9.5 MB (9474125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cc9c9a7b851c579ac8dac027ca82c6ee83b0f0c7e950503d59bd350badbe6c`  
		Last Modified: Tue, 12 Jan 2021 03:49:27 GMT  
		Size: 92.5 MB (92501570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:ea4f8715711afb573a6e3c2613975886ac7aed3d3f7c6681ee461a493bfcb1bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:fdb8539819660ff503bd662be2901cdce1b03fe1141c92883a60e05d46f58545
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2543079070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64888b637748e8242b8e2aacf412a234514184b731a8f2f54ea067b1563cd1ce`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:51:57 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:51:58 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:54:07 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:54:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d455d90e93f5eada528324775225d40a7a1550c6592b94e0ca492edbb3eecbd`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539e4779ae807fba7ee5490c9de973bcc5a2732e5cc8b7f151b95238051d9b9`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144a18fadb6c2512ef580ea9d52e5fb41995c189c297843fd2b58b66eee71dab`  
		Last Modified: Wed, 13 Jan 2021 19:02:24 GMT  
		Size: 107.3 MB (107302414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3bd53ab29546094935034aa7b475c582b0a5e7ebe1ad866ef2de8194745952`  
		Last Modified: Wed, 13 Jan 2021 19:01:53 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:4a147398f6f0e446f55a11aa0320c92e61fdb026e2cfe37c8eb966005e6e1888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:54139b747e8989c5b9dd1b782cedd068db26df94dffa3cd01a93fc10f510013c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5901999287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5700a05b11510e95fe0f03623b20428d2d71cf2b5b08735d2b66e1eefdb10e48`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:54:23 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 13 Jan 2021 18:54:24 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 13 Jan 2021 18:57:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:57:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a5352a2cb4c292314199884a957537c41ff1d8129b9b1b6ee38e5371cd7878`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb57a5b62ded9f8545dcc267b92de5d3ce66ab3b2faff3ee1149c238a66ae6`  
		Last Modified: Wed, 13 Jan 2021 19:02:42 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928d7681603fff97b6322d1e7e4fc7b114e4b5030782dfc407f159fa468cf3f6`  
		Last Modified: Wed, 13 Jan 2021 19:03:04 GMT  
		Size: 108.1 MB (108100699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16a97fd0203f542a9ba2737df2071b68283aa7fbcb59e222a94f1eadffba4f5`  
		Last Modified: Wed, 13 Jan 2021 19:02:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5`

```console
$ docker pull julia@sha256:1a1bb9b9d33e5df42f9d50aaaf9775d955bc49a24404ef54a0fa48875111732c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.5` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3`

```console
$ docker pull julia@sha256:1a1bb9b9d33e5df42f9d50aaaf9775d955bc49a24404ef54a0fa48875111732c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.5.3` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-alpine`

```console
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5.3-alpine` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
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
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5.3-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-buster`

```console
$ docker pull julia@sha256:2ef9304dd4d4e438cd5d4a2d0c98666049f96fa1cbd8ae7ff100d649a3186145
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.5.3-buster` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5.3-buster` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-windowsservercore-1809`

```console
$ docker pull julia@sha256:891d7b375b052c029653d919e37d317e55bb32267184facb59149d8d66a2e8ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.5.3-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5.3-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:94138add1cfcec70baf5c7b641984657c9c5013fa597d6afcef41075240cfcf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.5.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-alpine`

```console
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5-alpine` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
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
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.5-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-buster`

```console
$ docker pull julia@sha256:2ef9304dd4d4e438cd5d4a2d0c98666049f96fa1cbd8ae7ff100d649a3186145
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.5-buster` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:891d7b375b052c029653d919e37d317e55bb32267184facb59149d8d66a2e8ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.5-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:94138add1cfcec70baf5c7b641984657c9c5013fa597d6afcef41075240cfcf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:15ef2e799acfa365e408cf0222abcf8504fd35813a5e744363a16b5d5d02d2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0`

```console
$ docker pull julia@sha256:15ef2e799acfa365e408cf0222abcf8504fd35813a5e744363a16b5d5d02d2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6.0` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-beta1`

```console
$ docker pull julia@sha256:15ef2e799acfa365e408cf0222abcf8504fd35813a5e744363a16b5d5d02d2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6.0-beta1` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-beta1` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-beta1` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-beta1` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-beta1` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-beta1-buster`

```console
$ docker pull julia@sha256:8fa150d157edfb5db7a7210a54543ad00e07f7176815872fb51ad3a0d8b60049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6.0-beta1-buster` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-beta1-buster` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-beta1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-beta1-windowsservercore-1809`

```console
$ docker pull julia@sha256:80a475a2342c75adf9e59dc79579fe536d36b87b10b5ab32251016ab87343c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.6.0-beta1-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-beta1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:782ab30c2cac3cd09e14e4986c4998bcb67a3eed443a60cb271950353b000b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6.0-beta1-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-buster`

```console
$ docker pull julia@sha256:8fa150d157edfb5db7a7210a54543ad00e07f7176815872fb51ad3a0d8b60049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-buster` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.0-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:80a475a2342c75adf9e59dc79579fe536d36b87b10b5ab32251016ab87343c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.6.0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:782ab30c2cac3cd09e14e4986c4998bcb67a3eed443a60cb271950353b000b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:8fa150d157edfb5db7a7210a54543ad00e07f7176815872fb51ad3a0d8b60049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc`

```console
$ docker pull julia@sha256:15ef2e799acfa365e408cf0222abcf8504fd35813a5e744363a16b5d5d02d2df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6-rc` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc-buster`

```console
$ docker pull julia@sha256:8fa150d157edfb5db7a7210a54543ad00e07f7176815872fb51ad3a0d8b60049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6-rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:aa8f89abb0b5c46ddfbca2e09911df24031fe28db90bf9f99dbad7ac30e31ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151882800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bebd5c999f563adbc6b34c6b323ab3e79974c09fc720f401a1b174d1b61cf9e`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 09:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cdbeb670d2aea9af27ae96f4b872e04e3e64d67b526eaaa18a7e7448612156`  
		Last Modified: Tue, 12 Jan 2021 09:35:38 GMT  
		Size: 120.3 MB (120337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc-buster` - linux; 386

```console
$ docker pull julia@sha256:00dcee0556febc96ad6f0ddd9b64ffd16fae02e6045a3b9222bdbf3fd34113e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150402066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97f1ccb8152eb1403e8c93563d5ae32f5fb9dbf724822609960763c98062840`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 03:44:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:44:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f3f80667f6bfa62f82972d20808facdb1e190b3d4ff75fb5b28d62ee9b240e`  
		Last Modified: Tue, 12 Jan 2021 03:47:39 GMT  
		Size: 118.0 MB (118047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-rc-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:f22a16af5bd49dc0659933f7b51c6f33fc74a580ae3d619e6acee2ec18b7f6c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141105223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a78f73efbe0b162e375cccc08db4fd8e19bf54f865dac2e2653b438665ff97`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 02:57:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 02:57:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 02:57:12 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Tue, 12 Jan 2021 02:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30b214c7f544c6589a20104eaa6764eb368cadac5fa834b7454b747043e5a2b8' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='6f4a0d63c7bc69b5e649710c31affe7e39a554c895235df50eddc9d26bcc3910' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='de8c8e3560974196c09b4a01c91591ce4faf8c77daf080fb37b9e2759c5df29d' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='13f6192990d1c44039444707d8753d80b299c3fa05625ee9ca1680413ae344cd' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 02:59:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d681b73962d68385d038e19ad39019eac0c9fcc14f6dfab5b3e6e0517b015`  
		Last Modified: Tue, 12 Jan 2021 02:59:34 GMT  
		Size: 4.8 MB (4838144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea79d9e1b49ddbd0544722385165bc02d6ca5873d8f63cb9b17085f254afc0`  
		Last Modified: Tue, 12 Jan 2021 02:59:52 GMT  
		Size: 105.7 MB (105734242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:80a475a2342c75adf9e59dc79579fe536d36b87b10b5ab32251016ab87343c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.6-rc-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-rc-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:782ab30c2cac3cd09e14e4986c4998bcb67a3eed443a60cb271950353b000b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6-rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:80a475a2342c75adf9e59dc79579fe536d36b87b10b5ab32251016ab87343c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:c4a07b8709b8edc2eb6035e5e839878175ac4e51f3db67490abbe2cdf3527895
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2577184210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5ba706753cbc21efa935e8eda3c26526841c78f294b4139ccc7ee769b4f8c8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:40:24 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:42:49 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:42:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53296f463bbc81cde53c9b854c77bea62242ff4abe6927b0b2bb8eb10c25ef9f`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bedd67ba779a3bd2e7b051b72d9deccd1f9723b3a8c55c954e502e2a20bc406`  
		Last Modified: Wed, 13 Jan 2021 18:58:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd1af3201441f71d41bacf9ab926e34d58a1dc2e75e03a39f1c580632dee0c`  
		Last Modified: Wed, 13 Jan 2021 18:58:44 GMT  
		Size: 141.4 MB (141407517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d110e64b227c46bff80aff1835f75841dda8ecbd3583b2ac922469dc518979`  
		Last Modified: Wed, 13 Jan 2021 18:58:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:782ab30c2cac3cd09e14e4986c4998bcb67a3eed443a60cb271950353b000b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:ca6d233d1c24b1435a4659faadf4b7e3263d4384bf0d3890bbd42453a744dbec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5936108337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29dfcafd7448a557387412cfda782101f5dbdb0831468e6bbecde846a24c943`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:43:05 GMT
ENV JULIA_VERSION=1.6.0-beta1
# Wed, 13 Jan 2021 18:43:06 GMT
ENV JULIA_SHA256=f308a7b7e877a232a19d47d78b4bf55a974c9c24052ab867f346a151a8a91f90
# Wed, 13 Jan 2021 18:46:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:46:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8edbee3114fd4f6c283dad2b20cb56559683b6fa596af59e3e87a884dd0ef`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ad2d57e37f61be6f4633589f96e4b47baa4de556382c3d804f1358647c6e8`  
		Last Modified: Wed, 13 Jan 2021 18:59:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4368f3b79ea6d912f88eb2e80cb6c5710cdc944be91cb421d4cf8a0ba46cf2d7`  
		Last Modified: Wed, 13 Jan 2021 18:59:37 GMT  
		Size: 142.2 MB (142209753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65383cf11a2a7491ee22542208c02052e1efe83f7491ebf59a0b78f239f448`  
		Last Modified: Wed, 13 Jan 2021 18:59:06 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
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
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:2ef9304dd4d4e438cd5d4a2d0c98666049f96fa1cbd8ae7ff100d649a3186145
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:891d7b375b052c029653d919e37d317e55bb32267184facb59149d8d66a2e8ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:94138add1cfcec70baf5c7b641984657c9c5013fa597d6afcef41075240cfcf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
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
$ docker pull julia@sha256:09be7d53311af0dfae43abe0a6b98d35405718f8a531cec415bd48148fa45b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:14ce5514e14d328e7ecdd7dc4d2bfe1be700404db2e8f118283000f59da197a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112521703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791ac28996fca71fddde5c51ca9559f09750552bd5a7b56e1fd99fbc3b429ef`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 02 Feb 2021 23:19:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Feb 2021 23:19:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 02 Feb 2021 23:19:53 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 02 Feb 2021 23:20:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 02 Feb 2021 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114ff8a1a61ed37141133baeeaaa90e152979d15c5991f39c7b07cd3c3bd73a`  
		Last Modified: Tue, 02 Feb 2021 23:21:19 GMT  
		Size: 109.7 MB (109710382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:2ef9304dd4d4e438cd5d4a2d0c98666049f96fa1cbd8ae7ff100d649a3186145
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:1a1bb9b9d33e5df42f9d50aaaf9775d955bc49a24404ef54a0fa48875111732c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:e6a8487cba9efe82002e4ac04d1a6119c746f5f506b43345690f457409898e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144605135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb02260f0ed2b8dc9de0f941eeaace9caebbcbebeeb577115ad6635d2be2eb63`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:31:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 09:31:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 09:31:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 09:32:32 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 09:32:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 09:32:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32896747c5a7efad353da86892ecdc971a433890a13b829fdffe8a5614d6e2dc`  
		Last Modified: Tue, 12 Jan 2021 09:35:07 GMT  
		Size: 4.4 MB (4436955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0861f67cea5321a5e2ea3bb5653d9b41574a2133cde811e855039eeabd88e2c2`  
		Last Modified: Tue, 12 Jan 2021 09:36:21 GMT  
		Size: 113.1 MB (113060111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:50302434f6f4bf4d06f2bb39fdcdc49c7c62f8fd7cde93addbbe75ef300beada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135584959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9788aca5267e5fdca93d83b6e3955e8d3d61ecb96924b9a7f149bcaa7e773de0`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:46:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 11 Dec 2020 16:46:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 11 Dec 2020 16:46:47 GMT
ENV JULIA_VERSION=1.5.3
# Fri, 11 Dec 2020 16:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='3d6641b61b00415fa52a616a61bbd91dbbb1b4e6e9c61b7941710ed6ff720cb4' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 11 Dec 2020 16:47:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac498d66dc3580321c2af0a78454fe9f7c16f6a5ea0e4151133550b2dda48ce`  
		Last Modified: Fri, 11 Dec 2020 16:49:40 GMT  
		Size: 4.3 MB (4315197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c436a027dde049cd17c5ddabfc5137fd2ab2080c848e1e8ebb7ae383a03aff`  
		Last Modified: Fri, 11 Dec 2020 16:50:06 GMT  
		Size: 105.4 MB (105413571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:6b9227999d180138132a2c331a7b71f13430ea07e5b617bcf6667af36f927ce3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142423832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d5bb70b0b3507c1c75f305d22c24ba87e3bed114746456a4e492fc588e344`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Jan 2021 03:44:24 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 03:44:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Jan 2021 03:44:55 GMT
ENV JULIA_VERSION=1.5.3
# Tue, 12 Jan 2021 03:45:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='f190c938dd6fed97021953240523c9db448ec0a6760b574afd4e9924ab5615f1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1e8445eae896d347200b819b7a41778597ae15c314d9df080172eb868a42b628' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b265144f136dcaf2336b5abc8d18ae405ad5834de058a0338a4d020bede2fe47' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Jan 2021 03:45:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf6fa18d75742666732c7e69f4a782ecbf7dcc557faaeef0ae1d8abb397be0`  
		Last Modified: Tue, 12 Jan 2021 03:47:08 GMT  
		Size: 4.6 MB (4586370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343109c69a8121b255b962ab939a50f8ae17c343f06128a171332a3c8a0b81c7`  
		Last Modified: Tue, 12 Jan 2021 03:48:18 GMT  
		Size: 110.1 MB (110069471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:891d7b375b052c029653d919e37d317e55bb32267184facb59149d8d66a2e8ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull julia@sha256:e52df6a307ce481d3cdc2715487fbcd40364b18161b715d245fc3697b304ae5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572770569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c51ba5d91daad45091def17a7205f48385243b37cff94a800f7028b614d7eb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:46:19 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:46:20 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:48:32 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:48:35 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f41b333442914c47735f0a949c1988cbb2786c45589d9e4db720ad02f744d76`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5041ab13daa909297d004a59767baa9073235b9e833405cc1468b7caea7e6b`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf484d0366c12f9456f6dc2a22dbfc3f08fdec675e1a78b3be0e23ddbc3ca82`  
		Last Modified: Wed, 13 Jan 2021 19:00:40 GMT  
		Size: 137.0 MB (136993851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44efd2c91b6b603ecdd1556ca2b34978aa9291a0eba7f1a0302f1ab2293ba6bd`  
		Last Modified: Wed, 13 Jan 2021 19:00:04 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:94138add1cfcec70baf5c7b641984657c9c5013fa597d6afcef41075240cfcf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull julia@sha256:500b4767abffbc6a0a6f2435828c0be9bf3e6d90988de2492beaae0c819cc636
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5931699560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c29a3392dae8408d8ac48d68583c4631dfea52303d35edb3ca633d40457ed5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 18:48:46 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 13 Jan 2021 18:48:47 GMT
ENV JULIA_SHA256=5c5c5f8794747072296d33d6547977a61126c6283b449814fb6e8005fb282a59
# Wed, 13 Jan 2021 18:51:46 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 18:51:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6103aee463c5458e642be4f996245ff978b8a64c5463bf821f8a9606492dc`  
		Last Modified: Wed, 13 Jan 2021 19:01:03 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80382b4e32c15b2f1208cdd4bf597fb3da9377d1ea6685e7707f94d52b292ac5`  
		Last Modified: Wed, 13 Jan 2021 19:01:05 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e07178e83ced0a4280f9cbc750a424c807695e7ab673e8713a94ae3dab182`  
		Last Modified: Wed, 13 Jan 2021 19:01:32 GMT  
		Size: 137.8 MB (137800886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c6caa9c58da5bcf7a95a583af8858f935a15e03d6cd6a10eae93f18acc546`  
		Last Modified: Wed, 13 Jan 2021 19:01:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
