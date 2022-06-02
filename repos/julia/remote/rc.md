## `julia:rc`

```console
$ docker pull julia@sha256:c22367f359f39c165b7037de864aa1df2bf2719788d43e01cfa72a1cccd6b707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `julia:rc` - linux; amd64

```console
$ docker pull julia@sha256:ad82d0ac1eeb7fb0bdad81e3b7a9eced8b4c5126aa053c70ab2f112961959681
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178534442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3428f73ccfe1dde3e61a77375bd1ff94d1a679585ae76d8e544a7094d78817`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:22:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:22:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 05:22:07 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 05:22:07 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 18:32:59 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 18:33:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Jun 2022 18:33:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eda415c0e29e6a7b2336cfb8d64af2edf15ca42f3035042e9e9dc9d04e67740`  
		Last Modified: Sat, 28 May 2022 05:25:21 GMT  
		Size: 2.4 MB (2425947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a4bef474e869bc28914d4786d69fd9fa4088aa23e5d2b074560a3cbfd78e84`  
		Last Modified: Thu, 02 Jun 2022 18:36:10 GMT  
		Size: 144.7 MB (144729219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:09f65d856c6df826ce585dbba8b7475a8dc88ee449e4ca7ab1ccb6175acecb3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.5 MB (170489028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d883eb693437a964875bd8e29c6c109a529525aa317fe04ae7a92054f651fc32`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:34:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:34:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 02:34:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:34:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 17:57:00 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 17:57:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Jun 2022 17:57:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5009ca1e06d69bfe9ec7e7c510ef3712bb224c97f82fdaaa98effd93fabbe0e`  
		Last Modified: Sat, 28 May 2022 02:37:44 GMT  
		Size: 2.2 MB (2208675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b6c4dc27f85e1fddabdb5c0a9b4b4a06ffdde59264380ad6fbd27e325f9374`  
		Last Modified: Thu, 02 Jun 2022 17:59:19 GMT  
		Size: 138.2 MB (138214625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; 386

```console
$ docker pull julia@sha256:29841149a017c980e42b57ebac48b4f3045cc23ac3896bbb7ea5926898d932e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.4 MB (174444854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb31251963c7cb2e40d156cdd944962f9ff47f92f3aec0f1cdc2873faa9e606`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:34:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 03:34:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:34:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 17:42:37 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 17:43:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Jun 2022 17:43:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ab24c5119b700891a3f447f29ac0960077800cc5f71e2353786b09cc525fca`  
		Last Modified: Sat, 28 May 2022 03:37:42 GMT  
		Size: 2.3 MB (2324352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99633d9d235882e94a53348f4724fc8b7ab74e0c90b9439441fb4c64c02e336`  
		Last Modified: Thu, 02 Jun 2022 17:45:06 GMT  
		Size: 139.7 MB (139730181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.20348.707; amd64

```console
$ docker pull julia@sha256:983ea07e4107856574c5a3fa7e42a5af1c020a25baad219a7da0aa41146ef59a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2397543857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89017b68840a3d3234a1fe32e9127499e8816a76f17b5f00479921ba755f79e7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 02 Jun 2022 18:15:26 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 18:15:27 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-rc1-win64.exe
# Thu, 02 Jun 2022 18:15:28 GMT
ENV JULIA_SHA256=f739f4fb46030df00cbaea513afd427b436fc91b6fc6d7f4e437498cd16cc2aa
# Thu, 02 Jun 2022 18:17:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 02 Jun 2022 18:17:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f5fffbd70b57b4eec3fbfcd4f8a1288d24a392ae5e11a94add66fbbde1643`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3def9dba5937e7213b5246028e80bc8112e38fdaa13d0336909be43db1f64a8f`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76e08ee43498f0b5386766ce95caeecf9adc309147ee919b4e7dd88fc44b3c0`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f793c8c8f284d76cc82d62b369d42420fa1c250b3c105192ee91a0f56e737f`  
		Last Modified: Thu, 02 Jun 2022 18:23:45 GMT  
		Size: 160.0 MB (160001498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25069aeb4a7ae18df5f47c9be62dc83908c86664777b53db24058de33912ffe`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.17763.2928; amd64

```console
$ docker pull julia@sha256:edb09d5d94df484021a47f9fdceaa67eddb33e56c9107769f2387c750ce78ef9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2663963196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a43fd15941e51738a949a752caa2e9ec4410bd1beb592487ce9f68cf92c18030`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 02 Jun 2022 18:17:10 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 18:17:11 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-rc1-win64.exe
# Thu, 02 Jun 2022 18:17:12 GMT
ENV JULIA_SHA256=f739f4fb46030df00cbaea513afd427b436fc91b6fc6d7f4e437498cd16cc2aa
# Thu, 02 Jun 2022 18:19:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 02 Jun 2022 18:19:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06ad1a3153f9b28011cd85a894e69e79e44b7be3e1db7c3a6810c73bd1bdf7`  
		Last Modified: Thu, 02 Jun 2022 18:23:57 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc79f78a053aef2f9d97b9a63a58bbfe52c7a35ee59e763e13831a220777a7e9`  
		Last Modified: Thu, 02 Jun 2022 18:23:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07916e541bc9f3beb7cfa2523e47da15e639d6d0af1d919c78c428262e1b62e1`  
		Last Modified: Thu, 02 Jun 2022 18:23:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f934a5d1123b1c8fd970062e674c84184039ff09693b90bbb35f38bccde23c`  
		Last Modified: Thu, 02 Jun 2022 18:26:53 GMT  
		Size: 159.9 MB (159900234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0c3a9e5159747d5651607ff4c68e6641c48c8c5adf63d310a726928050fc15`  
		Last Modified: Thu, 02 Jun 2022 18:23:57 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
