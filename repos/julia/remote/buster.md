## `julia:buster`

```console
$ docker pull julia@sha256:956a0a0e87f86581b9b00d94d8fe48980302eac2bb218824050439446e2211ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:48937060ff93ae448b072263d61ee808be1594185bbaa9fadced6db42be29bb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.3 MB (153286261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:707777fd72fc7c14d1d3a6935c33af074d56a91f2da13e6593a82cf6a0a9d6fc`
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
# Thu, 02 Dec 2021 09:43:53 GMT
ENV JULIA_VERSION=1.6.4
# Thu, 02 Dec 2021 09:44:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Dec 2021 09:44:11 GMT
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
	-	`sha256:ab0e35e44e68ba9806eebf32f56ea1f3330676ef3c8e13e26b494a91936e4979`  
		Last Modified: Thu, 02 Dec 2021 09:48:30 GMT  
		Size: 121.7 MB (121673990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:2d765975c8a4cfa884b10d2ba0a9ce8b215d11a4fba8b85c821a8a5c60a2aba8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139468568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e00876aecfc2bd801918c448805ee9b2675b8b75222c10ca490c908c5c3706`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:21 GMT
ADD file:7b30d743b30e84b21888f23cb7f266caba09db98b7a4c8800abebcf03d28c01d in / 
# Thu, 02 Dec 2021 09:06:22 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 15:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 15:55:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 02 Dec 2021 15:55:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 15:55:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Dec 2021 15:58:07 GMT
ENV JULIA_VERSION=1.6.4
# Thu, 02 Dec 2021 15:58:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Dec 2021 15:58:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2aa85085c98821a25a3058f7fc2c6427064f2228ea8eac904e9e7db4dbdaa01a`  
		Last Modified: Thu, 02 Dec 2021 09:22:26 GMT  
		Size: 22.8 MB (22754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ada6a5e8fe302e1e9ef466d0da0cc87d2339e25533cb08a044bd660165fa6`  
		Last Modified: Thu, 02 Dec 2021 16:04:23 GMT  
		Size: 3.8 MB (3806048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661f743504ec29bd6b040e2203b21eccc28169a65d7ce2e943132a00df724a7d`  
		Last Modified: Thu, 02 Dec 2021 16:08:39 GMT  
		Size: 112.9 MB (112908155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:d9bdb79d807b1654c98525102b535d4d0b94804df9d95143b2d6cd928edf9816
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.5 MB (145549008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba06cb918bf1e3309fb0182c522a5a2fcd6484af3fa337a83bbbb759a6b9b0b7`
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
# Thu, 02 Dec 2021 10:21:44 GMT
ENV JULIA_VERSION=1.6.4
# Thu, 02 Dec 2021 10:21:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Dec 2021 10:22:00 GMT
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
	-	`sha256:e39b2bba91454eb6c5b227df7159f1129ae22ba1e4c93bf637397e8e08773260`  
		Last Modified: Thu, 02 Dec 2021 10:25:41 GMT  
		Size: 115.3 MB (115287663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:18d11042d971fa86492da10aaea4ad5d6b010ee4ae5ac4bc331a86b4c28868fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.7 MB (151748606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db7cd07be651955a21f44d595016952c5dd5047117328cc99acbe449fb897c2`
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
# Thu, 02 Dec 2021 09:21:02 GMT
ENV JULIA_VERSION=1.6.4
# Thu, 02 Dec 2021 09:21:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Dec 2021 09:21:23 GMT
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
	-	`sha256:f1086110b34bf523c08a9d87d044157c71b826c94971570a08389e14ecc465d7`  
		Last Modified: Thu, 02 Dec 2021 09:26:06 GMT  
		Size: 119.3 MB (119333121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
