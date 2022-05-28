## `julia:buster`

```console
$ docker pull julia@sha256:fe01cd0a88dd582bf5d1da86c1f2e3a2a3ff20c736318cb3f22a8f6e38732001
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:000d0b3eae0d10d965fe359e36b413c29bb96469f4eebf47db992153809ee36e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163985114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af9624cde209adce0ccd3815b5e2dfb7348a8c4c26cd8515c2f85a282b4ef3b`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:22:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:22:42 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 05:22:42 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 05:22:42 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 May 2022 05:23:27 GMT
ENV JULIA_VERSION=1.7.3
# Sat, 28 May 2022 05:23:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.3-linux-x86_64.tar.gz'; 			sha256='9b2f4fa12d92b4dcc5d11dc66fb118c47681a76d3df8da064cc97573f2f5c739'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.3-linux-armv7l.tar.gz'; 			sha256='e9de15c56b9b62727c69d10da4b8e90fa6609d2e94e9cfb9f99128dfb59a8677'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.3-linux-aarch64.tar.gz'; 			sha256='d9e8b342c80ad1371520ed6d11f55b78aa60746737fbf57ecafd6a23b52dd71d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.3-linux-i686.tar.gz'; 			sha256='c1e1a4f9a53affee269c7e740cb8bd46740f9021414459c3ab3bb2c540d9d499'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 May 2022 05:23:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c15273495b3dd9df3800e0ff83cd143d969508a99b5fe7af8cf49c967a09939`  
		Last Modified: Sat, 28 May 2022 05:25:56 GMT  
		Size: 4.5 MB (4468214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555c41c3aeca24b9848c3303750879eb2bcd34adec2803c615c47926f6b1ce0c`  
		Last Modified: Sat, 28 May 2022 05:27:29 GMT  
		Size: 132.4 MB (132376756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a1c305a65accaff65e569418b94830571253f022d5bd709e556d61d8bf66f7aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147899499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab59c786c08bea1713fa321252788cfc2257b864a1712fce7d50f55aac9d5db`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 01:00:54 GMT
ADD file:c89d47099a38749a424760d9c7d3a6e982089455ba9d04140db15ba9eb4cdda1 in / 
# Sat, 28 May 2022 01:00:55 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:38:41 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 07:38:42 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 07:38:42 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 May 2022 07:38:43 GMT
ENV JULIA_VERSION=1.7.3
# Sat, 28 May 2022 07:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.3-linux-x86_64.tar.gz'; 			sha256='9b2f4fa12d92b4dcc5d11dc66fb118c47681a76d3df8da064cc97573f2f5c739'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.3-linux-armv7l.tar.gz'; 			sha256='e9de15c56b9b62727c69d10da4b8e90fa6609d2e94e9cfb9f99128dfb59a8677'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.3-linux-aarch64.tar.gz'; 			sha256='d9e8b342c80ad1371520ed6d11f55b78aa60746737fbf57ecafd6a23b52dd71d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.3-linux-i686.tar.gz'; 			sha256='c1e1a4f9a53affee269c7e740cb8bd46740f9021414459c3ab3bb2c540d9d499'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 May 2022 07:39:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e41117292dc8c199b63ae1ec4485358841dbcba68dcbd13f379b66182efe832e`  
		Last Modified: Sat, 28 May 2022 01:16:58 GMT  
		Size: 22.7 MB (22748097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700e2b9ac9f610ff491376f8749b1cd7f928cf7c5cb8b68e67acd681ce6c5d59`  
		Last Modified: Sat, 28 May 2022 07:44:20 GMT  
		Size: 3.8 MB (3811311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b856efebc4c9f078085d923a0827a4d184281ec4417919860f4b2caa3162e11`  
		Last Modified: Sat, 28 May 2022 07:45:37 GMT  
		Size: 121.3 MB (121340091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0ca95193c78327c2767efa7ef863fd8a25ae9f1c244eedee267431fc4fc380d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.5 MB (155537532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a629a1e8bb2cf0978c448189ce60e4c37e3425aecdd01f91ba2261c707437f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:34:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 02:34:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:34:58 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 May 2022 02:35:49 GMT
ENV JULIA_VERSION=1.7.3
# Sat, 28 May 2022 02:36:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.3-linux-x86_64.tar.gz'; 			sha256='9b2f4fa12d92b4dcc5d11dc66fb118c47681a76d3df8da064cc97573f2f5c739'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.3-linux-armv7l.tar.gz'; 			sha256='e9de15c56b9b62727c69d10da4b8e90fa6609d2e94e9cfb9f99128dfb59a8677'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.3-linux-aarch64.tar.gz'; 			sha256='d9e8b342c80ad1371520ed6d11f55b78aa60746737fbf57ecafd6a23b52dd71d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.3-linux-i686.tar.gz'; 			sha256='c1e1a4f9a53affee269c7e740cb8bd46740f9021414459c3ab3bb2c540d9d499'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 May 2022 02:36:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc371f868dbfc86f00f21fb937bee8a4ad6005b956e2af368cdb394d46bd9d6`  
		Last Modified: Sat, 28 May 2022 02:38:20 GMT  
		Size: 4.3 MB (4346881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd3a42aaea9b9c24154069477c71f2dcfa646053c7cf11ad958be2d5d6be2a`  
		Last Modified: Sat, 28 May 2022 02:39:50 GMT  
		Size: 125.3 MB (125276618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:eb3beb1b543c6a846525b093f805d65caf7d14c5fd74e15da13006b36973c502
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160616039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81df7febc2d58bfd80643ef6adf6bc7c3fe2d86ce3b639c01e638d9459c750e9`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:34:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:34:41 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 03:34:42 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:34:43 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 28 May 2022 03:35:39 GMT
ENV JULIA_VERSION=1.7.3
# Sat, 28 May 2022 03:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.3-linux-x86_64.tar.gz'; 			sha256='9b2f4fa12d92b4dcc5d11dc66fb118c47681a76d3df8da064cc97573f2f5c739'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.3-linux-armv7l.tar.gz'; 			sha256='e9de15c56b9b62727c69d10da4b8e90fa6609d2e94e9cfb9f99128dfb59a8677'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.3-linux-aarch64.tar.gz'; 			sha256='d9e8b342c80ad1371520ed6d11f55b78aa60746737fbf57ecafd6a23b52dd71d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.3-linux-i686.tar.gz'; 			sha256='c1e1a4f9a53affee269c7e740cb8bd46740f9021414459c3ab3bb2c540d9d499'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 28 May 2022 03:35:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398b9492cc24e1bb8000f38491e8dd66b801d68bbaab87bba3b1ab764eb437aa`  
		Last Modified: Sat, 28 May 2022 03:38:14 GMT  
		Size: 4.6 MB (4616185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6417f46e0a81129c170baec70f3bd520efd4fe8b336babfb438de62f1e94cbe`  
		Last Modified: Sat, 28 May 2022 03:39:36 GMT  
		Size: 128.2 MB (128200282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
