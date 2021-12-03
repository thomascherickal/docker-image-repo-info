## `julia:buster`

```console
$ docker pull julia@sha256:8654ff9ceabe29877d424759ee41fe4b1f41f8462502db9d601f6629b875bcd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:1de868195d1a814c724d1b7cc9875b2171e49523fa4921972e9b02d1c4f061ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.1 MB (164127401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba43ba79b5b2fa896e56e492e440b17848624924d7e60fcd960e254cd6cd3927`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:42:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:42:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 02 Dec 2021 09:42:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 09:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Dec 2021 20:32:27 GMT
ENV JULIA_VERSION=1.7.0
# Fri, 03 Dec 2021 20:32:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.0-linux-x86_64.tar.gz'; 			sha256='7299f3a638aec5e0b9e14eaf0e6221c4fe27189aa0b38ac5a36f03f0dc4c0d40'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.0-linux-aarch64.tar.gz'; 			sha256='85a93659ef588b7ee9e3eb2ee1e8b1ba8bb200adc4389afed054be44e51e6540'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.0-linux-i686.tar.gz'; 			sha256='e4498be9c2449791093938e8e4f6a93a708d2a8bf27605c835c7409c0a57695d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Dec 2021 20:32:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20759da86ee815c76ac66ee463388da4394f7392c03224943a2bd16dc7465c61`  
		Last Modified: Thu, 02 Dec 2021 09:46:46 GMT  
		Size: 4.5 MB (4458542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa529cafc530b5c4af955e8e2dac098aa10e848f86893eb66299a3ad6033a63`  
		Last Modified: Fri, 03 Dec 2021 20:36:45 GMT  
		Size: 132.5 MB (132515130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:336cb896ae999604c58943889b743cabe1686b69ea014311c42da1abf6aa4f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155903798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f23960713543716c2ad395bd8af435c622bcd9b4148a97fa098640485611af`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:20:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 10:20:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 02 Dec 2021 10:20:55 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 10:20:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Dec 2021 16:38:30 GMT
ENV JULIA_VERSION=1.7.0
# Fri, 03 Dec 2021 16:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.0-linux-x86_64.tar.gz'; 			sha256='7299f3a638aec5e0b9e14eaf0e6221c4fe27189aa0b38ac5a36f03f0dc4c0d40'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.0-linux-aarch64.tar.gz'; 			sha256='85a93659ef588b7ee9e3eb2ee1e8b1ba8bb200adc4389afed054be44e51e6540'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.0-linux-i686.tar.gz'; 			sha256='e4498be9c2449791093938e8e4f6a93a708d2a8bf27605c835c7409c0a57695d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Dec 2021 16:38:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613768401ba4c98b7337eb641463cbd04d29d049c55cf47a4a732e5d16c6aa37`  
		Last Modified: Thu, 02 Dec 2021 10:24:14 GMT  
		Size: 4.3 MB (4338201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada7514678c27e5b9f100b5592999eb47922ea72db97c81f81418b5e6c6aa549`  
		Last Modified: Fri, 03 Dec 2021 16:41:10 GMT  
		Size: 125.6 MB (125642453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:6bc17f6e123e101929161a8e67d663644969aabd0248224949638ad252200a34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161067535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53fb7fe2bf06607e7cbf03841302b886b4e49515b81cd3dcb86642638a17db49`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:19:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:19:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 02 Dec 2021 09:19:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 09:20:00 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Dec 2021 11:57:22 GMT
ENV JULIA_VERSION=1.7.0
# Fri, 03 Dec 2021 11:57:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.0-linux-x86_64.tar.gz'; 			sha256='7299f3a638aec5e0b9e14eaf0e6221c4fe27189aa0b38ac5a36f03f0dc4c0d40'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.0-linux-aarch64.tar.gz'; 			sha256='85a93659ef588b7ee9e3eb2ee1e8b1ba8bb200adc4389afed054be44e51e6540'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.0-linux-i686.tar.gz'; 			sha256='e4498be9c2449791093938e8e4f6a93a708d2a8bf27605c835c7409c0a57695d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Dec 2021 11:57:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610c1c092d2a055f47d0a8f69b9a68445f7be8dd96e7cb88a4987b4594b06e10`  
		Last Modified: Thu, 02 Dec 2021 09:24:11 GMT  
		Size: 4.6 MB (4610923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449dabd2d773251d9f33948c89c9e48edf3d7b67efbf2531f849bfbabd8c5676`  
		Last Modified: Fri, 03 Dec 2021 12:00:52 GMT  
		Size: 128.7 MB (128652050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
