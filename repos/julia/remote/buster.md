## `julia:buster`

```console
$ docker pull julia@sha256:cfffecf4853bf51b8c4f27fb441c6b51c047a299960c3932011f3ecdfb757d07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:2001537187ae5003d5f4e138b8edd41d7cd05f2973e6946e0bc630f0bbaa85eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.1 MB (164088646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b2ca4292da40be51b5d57d8cb79160d98811edd5fdfdd1960bf4e2867eeba4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:54:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 09:54:07 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 09:54:07 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 09:54:52 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 09:55:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 09:55:08 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3430f6205326a5eb5f6e5e3694bbbb6d8a4a05e8a4b5beb527c024e7b6025826`  
		Last Modified: Wed, 20 Apr 2022 09:57:18 GMT  
		Size: 4.5 MB (4468077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eefe81d59e17e9cf23846fb4338a3969bc4d372bbab44f66ad7b1176140f7f1`  
		Last Modified: Wed, 20 Apr 2022 09:58:49 GMT  
		Size: 132.5 MB (132479905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:bf5ac46cbaf23fa14329716d2fb373908fdb0c4ea2167bcd86808009a0572c09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.4 MB (147421767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30af49f9f75031fb56998fe22b3ccea4d361cd3ecad3bf2bcbceaee1ab65174`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:37:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:37:10 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 21:37:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 21:37:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 21:37:11 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 21:37:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 21:37:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f36d41cea61458b4069b3d2f8705c9f1eba88d7251ce085b0f5c5e1c3e342b`  
		Last Modified: Wed, 20 Apr 2022 21:42:45 GMT  
		Size: 3.8 MB (3811220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85874fb01a65fec705d66bb07c16188ca61af792fb9ab79bc9015b902a67f23`  
		Last Modified: Wed, 20 Apr 2022 21:44:04 GMT  
		Size: 120.9 MB (120862682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:cf00105d52f92687571a02bae122f85bf14e6f7e49c1cf2e8938b09a313ce869
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156201170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaa9fcab2c0c545aea57d6a639d7ccf39a290cad01a69a79dc05bd66b88cca4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:27:55 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 09:27:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 09:27:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 09:28:46 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 09:29:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 09:29:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f8ef523e4215a9d657fd62acd42b636d676969f9ba4ef55f42aed1286f3532`  
		Last Modified: Wed, 20 Apr 2022 09:31:09 GMT  
		Size: 4.3 MB (4346836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8fb3369a12bf66c6f22ee349f69960c41ddb69d3048728cff8f203e5d3a3c1`  
		Last Modified: Wed, 20 Apr 2022 09:32:41 GMT  
		Size: 125.9 MB (125945985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:3819dec0af3656f517775129679dee744f9cf500ec2479abd610cba059b13f49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.8 MB (160833425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356bf533f07a7f462c8035823b763f029c62a5a10303fa3c58d01c346d25dd6b`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:42:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:42:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 20 Apr 2022 12:42:30 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 12:42:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 20 Apr 2022 12:43:29 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 20 Apr 2022 12:43:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.7/julia-1.7.2-linux-x86_64.tar.gz'; 			sha256='a75244724f3b2de0e7249c861fbf64078257c16fb4203be78f1cf4dd5973ba95'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.7/julia-1.7.2-linux-armv7l.tar.gz'; 			sha256='837c93adf75a3e981eacf35f24f1d95cd2e4d9c490b84befd3865b2d558b730c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.7/julia-1.7.2-linux-aarch64.tar.gz'; 			sha256='69fd58b1e8f6f8a72053dcbeab2d2882258fe372a91c7287d38b9c217885821a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.7/julia-1.7.2-linux-i686.tar.gz'; 			sha256='f5f8e6cbaf0acd473a5e13c23c80f0672207eb86408178fec221f4f7fb88f6d1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 20 Apr 2022 12:43:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c842a4ef0d0344fa2f69ba36819a9dc37046e5798539e879300e6ff4966d996`  
		Last Modified: Wed, 20 Apr 2022 12:45:59 GMT  
		Size: 4.6 MB (4615956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8824cab8fd2d28feebeac2927939997121dd71f450be5d22f4f7ebd1b72fa3`  
		Last Modified: Wed, 20 Apr 2022 12:47:25 GMT  
		Size: 128.4 MB (128417644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
