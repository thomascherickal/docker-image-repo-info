## `julia:rc-buster`

```console
$ docker pull julia@sha256:cd6a88175a00141f90fddb8c79c53727cfb517510e178ee9aa23a4437aea70cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:dbdc0e4b8d529d277fa372ffcfa38e25d74d096804e0c1929f216c6070cfa62f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176338728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c6755e3803800da1b236469801ce205c965d3fa566a5a0b9c4022e4f8ddfb82`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:48:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Jun 2022 03:48:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 03:48:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Jun 2022 03:48:46 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 23 Jun 2022 03:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Jun 2022 03:49:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b048d90a912a30e070c32b2a0684599a11aa8b964ab322a5f91ddeb4e86d02`  
		Last Modified: Thu, 23 Jun 2022 03:52:04 GMT  
		Size: 4.5 MB (4468159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7ea28a6191cfa2e37fa37c5520b7c6945fc699d91c99bc7cbcd2ee7cbf4871`  
		Last Modified: Thu, 23 Jun 2022 03:52:25 GMT  
		Size: 144.7 MB (144730526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:45a0cd1944ecb8b135b8b7707da9d05908243982ada9e19db1dc7d88d1cc7dcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.5 MB (168477805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:285162bc8631fc1966fe363074722837cd61e3d290c646850866df1a0714e2d0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:08 GMT
ADD file:e491c8ce913289e0c673bd14014c5506cca7b78575aa5c8303ec856525209505 in / 
# Thu, 23 Jun 2022 00:41:09 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 15:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:06:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Jun 2022 15:06:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 15:06:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Jun 2022 15:06:47 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 23 Jun 2022 15:07:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Jun 2022 15:07:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d8b55b2b6839f70c2ed0662b18f4d9724108500136dfd03e999a5f91c815984b`  
		Last Modified: Thu, 23 Jun 2022 00:48:15 GMT  
		Size: 25.9 MB (25914029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9ba8e53f33e8d2b281278e051d614098d90e000b4b13aa387d9f26ad5d3060`  
		Last Modified: Thu, 23 Jun 2022 15:10:11 GMT  
		Size: 4.3 MB (4346873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e93514c7abe1bc4baaad9e377ec6388c3cfb74dc2dd3a44b972b901b21fa9d7`  
		Last Modified: Thu, 23 Jun 2022 15:10:31 GMT  
		Size: 138.2 MB (138216903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; 386

```console
$ docker pull julia@sha256:f9efea0209569c717fbe18eb8b0fc33c3fd3cbebf826bc71f2d9b7ad38cb211f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.2 MB (172154646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8cf50f33a9920139ef9eb1ea95fce79e167371f02a0f7c14b42e2713f41f07`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:59 GMT
ADD file:d4d6ebbe6e038ac58e266fb07bee755ccccf597fb15b3e8264165279e8fbed3b in / 
# Thu, 23 Jun 2022 00:40:00 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:37:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Jun 2022 03:37:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 03:37:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Jun 2022 03:37:59 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 23 Jun 2022 03:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Jun 2022 03:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e8877ae0470a67233ffd6b1ee842fc356ff46b5b3c594a02395801f85ccec7b4`  
		Last Modified: Thu, 23 Jun 2022 00:47:36 GMT  
		Size: 27.8 MB (27799542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7b3a523a6765be51fb1f11e32b115c0f31d690bc1a9cee6c6f5231db7b0fa7`  
		Last Modified: Thu, 23 Jun 2022 03:41:38 GMT  
		Size: 4.6 MB (4616134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07fe757bf4cc7a5f4192d37cc92bc0d4087506ee7069b9f4788253c883007d6`  
		Last Modified: Thu, 23 Jun 2022 03:41:56 GMT  
		Size: 139.7 MB (139738970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
