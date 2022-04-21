## `julia:latest`

```console
$ docker pull julia@sha256:f69c5ccac101532e873a1166dff43906d12a1790ef9c687f6a4964624d6b058d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:2808b87dbf5c43ab2bb8dde9a0671a1aea1e36f7b546c9d057cd5108e017ac75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166285075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada80b2c423f730d5c215493de185e05f1dc45464e6366499eff1f4029228191`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:53:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:53:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 09:53:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 09:53:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 09:54:32 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 09:54:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 09:54:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0100a9853fd9d686ddda0af774ad31239eeede11b292a1e12bcbccc8129d80`  
		Last Modified: Wed, 20 Apr 2022 09:56:45 GMT  
		Size: 2.4 MB (2425643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0da1dd0a48f88dc7db33b189abfa2f30ab69ba13cf9e6b91864468163a58e46`  
		Last Modified: Wed, 20 Apr 2022 09:58:13 GMT  
		Size: 132.5 MB (132480453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:85175363e2d7ee9bb02b516441bde4c9dbb3e6907ca973fe5a44ea05a243da7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149652304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a7225b6b44cc767f6d432df70a96012fedaaa0f028679bddb8ca9cb9fa193d`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:35:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:35:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 21:35:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 21:35:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 21:35:46 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 21:36:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 21:36:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8c5af8dafe291ed25bcf3c57821bc2e53d314d0bb413cfbad82bf3037336b1`  
		Last Modified: Wed, 20 Apr 2022 21:41:10 GMT  
		Size: 2.2 MB (2227657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bff13b662acbb58ad5862e97628b21fc2df6b690897140622f4afbdcd6d7488`  
		Last Modified: Wed, 20 Apr 2022 21:42:23 GMT  
		Size: 120.8 MB (120848889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:3c6fcb5e739b51c2354f8db3e9de9d56ec5317fa7172c14101b45b5d0833468c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158204344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d700d2a813ec340994c4c5471d8650321b61aa8e5d3683d0846a34766ea5adfc`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:27:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:27:17 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 09:27:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 09:27:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 09:28:18 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 09:28:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 09:28:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cf6e0803d61e6110b0bd7486df54e14716d73c0eec66517515d79c4148c6ae`  
		Last Modified: Wed, 20 Apr 2022 09:30:36 GMT  
		Size: 2.2 MB (2208545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc3c43f05096b107d9ea4a8fde86cfec266efd063e814ba778665f2094d0b1a`  
		Last Modified: Wed, 20 Apr 2022 09:32:04 GMT  
		Size: 125.9 MB (125929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:b070db94db5d2c4bc807bdaf7d6be9b5831e54d7af7aaa55653c5537c0c09297
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163125640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d1fcf2bd4218b4b235dd0ba11c83b51692ceb64c17f588052c585aa0f82126`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:41:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:41:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 12:41:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 12:41:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 12:42:59 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 12:43:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 12:43:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525ea710908f0a668bcc31400b957ce8f7af76eec328726d9a77ba1a86f8cc`  
		Last Modified: Wed, 20 Apr 2022 12:45:29 GMT  
		Size: 2.3 MB (2324084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1999a3b206f48c122703c65a760fec3f14aaeb5346d94ab9a4a60c2ecd69fc`  
		Last Modified: Wed, 20 Apr 2022 12:46:45 GMT  
		Size: 128.4 MB (128411959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.643; amd64

```console
$ docker pull julia@sha256:a67ee0bc1796d3b88b6eb1907645c78c5c98021877f089e27b3fea5553d92de7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371985446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e48fbaa8e05d2b231daea2643abaeb90dcfdb05af2a6ad090b4441c6487b3`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 14:22:15 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 13 Apr 2022 14:22:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.2-win64.exe
# Wed, 13 Apr 2022 14:22:17 GMT
ENV JULIA_SHA256=bede21e00130c2dcb6973a968b7ed43c35d69712008a95bb08d5536d3c9e2585
# Wed, 13 Apr 2022 14:23:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 14:23:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95aa4757a8ca2ba122a9010f5511afc983949bf55af13dab23e4c23313258b44`  
		Last Modified: Wed, 13 Apr 2022 14:34:09 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dba6186b9891cf7977432c78227c47dceb98223377547431aeacd7dca66349`  
		Last Modified: Wed, 13 Apr 2022 14:34:09 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b01c01ee3ee96c9823d27b9971f57954f451c34dc38cf96432e02c0ccb2f8a`  
		Last Modified: Wed, 13 Apr 2022 14:34:09 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30299afe7421f599b389a6d1454b182a4ca477bfb6c522384f29efef75af44ca`  
		Last Modified: Wed, 13 Apr 2022 14:36:53 GMT  
		Size: 145.0 MB (145023535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fb76d7a8a5b4032abe5d60ec1df2bfe646dbd3cdf10dd03b5b6b0611e57578`  
		Last Modified: Wed, 13 Apr 2022 14:34:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull julia@sha256:e1707a8b9c5f6cbb187d6f301bb7e08b105f2e5a0db4484ebe78c74e21edcc86
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2860700176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4f1a89e413ccc9f54a2744e992dda66ce478f20c65433190ec228ec462e5a69`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 14:24:01 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 13 Apr 2022 14:24:02 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.2-win64.exe
# Wed, 13 Apr 2022 14:24:03 GMT
ENV JULIA_SHA256=bede21e00130c2dcb6973a968b7ed43c35d69712008a95bb08d5536d3c9e2585
# Wed, 13 Apr 2022 14:26:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 14:26:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8367fe65c9f43984631ec180d79533f9391ee49402de4b0c4938c375b426f0f0`  
		Last Modified: Wed, 13 Apr 2022 14:37:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4dcdff66560c943c0ed2cee02b6b96df6933617488a3b225db38a71836a12`  
		Last Modified: Wed, 13 Apr 2022 14:37:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b2e9c75af4a34fa450aff47db1683ca0be784980283b4f5587918618910d2e`  
		Last Modified: Wed, 13 Apr 2022 14:37:09 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f1c1a72c15610b7dd5c103a158cdfaf6804f1266064e54b19f259bebd0cfae`  
		Last Modified: Wed, 13 Apr 2022 14:37:43 GMT  
		Size: 144.8 MB (144772902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5f0f5d7d40b71a4e04b1bcefe63729d89c2ece8caeb9291eb573d37bcff32e`  
		Last Modified: Wed, 13 Apr 2022 14:37:09 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
