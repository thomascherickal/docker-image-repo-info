<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rust`

-	[`rust:1`](#rust1)
-	[`rust:1.40`](#rust140)
-	[`rust:1.40.0`](#rust1400)
-	[`rust:1.40.0-alpine`](#rust1400-alpine)
-	[`rust:1.40.0-alpine3.10`](#rust1400-alpine310)
-	[`rust:1.40.0-buster`](#rust1400-buster)
-	[`rust:1.40.0-slim`](#rust1400-slim)
-	[`rust:1.40.0-slim-buster`](#rust1400-slim-buster)
-	[`rust:1.40.0-slim-stretch`](#rust1400-slim-stretch)
-	[`rust:1.40.0-stretch`](#rust1400-stretch)
-	[`rust:1.40-alpine`](#rust140-alpine)
-	[`rust:1.40-alpine3.10`](#rust140-alpine310)
-	[`rust:1.40-buster`](#rust140-buster)
-	[`rust:1.40-slim`](#rust140-slim)
-	[`rust:1.40-slim-buster`](#rust140-slim-buster)
-	[`rust:1.40-slim-stretch`](#rust140-slim-stretch)
-	[`rust:1.40-stretch`](#rust140-stretch)
-	[`rust:1-alpine`](#rust1-alpine)
-	[`rust:1-alpine3.10`](#rust1-alpine310)
-	[`rust:1-buster`](#rust1-buster)
-	[`rust:1-slim`](#rust1-slim)
-	[`rust:1-slim-buster`](#rust1-slim-buster)
-	[`rust:1-slim-stretch`](#rust1-slim-stretch)
-	[`rust:1-stretch`](#rust1-stretch)
-	[`rust:alpine`](#rustalpine)
-	[`rust:alpine3.10`](#rustalpine310)
-	[`rust:buster`](#rustbuster)
-	[`rust:latest`](#rustlatest)
-	[`rust:slim`](#rustslim)
-	[`rust:slim-buster`](#rustslim-buster)
-	[`rust:slim-stretch`](#rustslim-stretch)
-	[`rust:stretch`](#ruststretch)

## `rust:1`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40.0` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-alpine`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.40.0-alpine` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-alpine3.10`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.40.0-alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-buster`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40.0-buster` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-buster` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-slim`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40.0-slim` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-slim-buster`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40.0-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-slim-stretch`

```console
$ docker pull rust@sha256:6dbd1450defc06557513c6ad040f948f25123065779ee697b611254d4d500daf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40.0-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:57c6607fec3c2bfebc517cb9c13321aee87cfd84bace6f53bddbb23c15452b77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189328904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e94d78b219741c33f7ca91069f2f418bd15960e08c8ac3f31be062ac60551fbb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:37:12 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a808f9be53ad3051a0da3ba8c2600cba69684fd510f3fc12d59be3902e4e890`  
		Last Modified: Thu, 19 Dec 2019 23:40:16 GMT  
		Size: 166.8 MB (166804332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:96d44debbfd641d7873d11242e287bfba85fd21ae03e83c6eb2a0b27bf55d4fc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162934818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d1807641c5badabb356a369f86b0ec894ccbd0932211ac957dbe7a973de4e3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:23:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbdd2d07539c94add88be67e07030cdbd1863504d08306bd60b7f60d17d1d1d`  
		Last Modified: Sat, 28 Dec 2019 15:27:42 GMT  
		Size: 143.6 MB (143623231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:a1ef6c8c6d5504d56fd9f67c866ace7ad1b26f02a11a3678ad971e163f9360ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164549005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048c98f570a1ff655c5340bd5b5c6c1c90783447553197e411d6ed34e205782e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:34:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b832e63d71815acfddc8f292e3348c05ee1643280093ea87850ed9cf21a03df`  
		Last Modified: Fri, 20 Dec 2019 00:39:34 GMT  
		Size: 144.2 MB (144163246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:51de05adbfe450e2f42058374d96259cf450476b62f8fabe8fde826baaf66cb9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210290258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1e3bd06388aaad6f6f6d663b16684cd9a7aed0e8e37c6cf538bbd239d9daca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:05 GMT
ADD file:d43798bcf0e72b342c261b8585dde072d9363d19fab4b8d9f08f15db189f287b in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:39:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2cb401c016d2f9802d5ef9cf6c6dc07251e9f87757a0de0a8df318fb7f00385c`  
		Last Modified: Sat, 28 Dec 2019 04:47:36 GMT  
		Size: 23.2 MB (23152142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e7005a402b4f68ea5da5d5fbc8e568f31de042b0c63a48dea6f837fc2a4b4`  
		Last Modified: Sat, 28 Dec 2019 19:43:42 GMT  
		Size: 187.1 MB (187138116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40.0-stretch`

```console
$ docker pull rust@sha256:8b678d1ce48cb057ac19cadd05162f40d80e72550153176984f604efbede66e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40.0-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8799cee901791082ca011eae1eb30fd62166fee80f38284e46c28dc764f5cdf5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.3 MB (454337046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5302f1b5dabd05a5ad5f9331511d3c230d2d4963c6e168f72857636e7beabf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:15:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:36:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:07 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9577c0793430759082b98068eb2884638a34fa46ca481099e93cfc38d4ebfe`  
		Last Modified: Sat, 23 Nov 2019 00:21:35 GMT  
		Size: 214.8 MB (214841433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1501da54344da67a16aa924db62c0d8f2adda671b60360c046fa04bc9f6e6ba`  
		Last Modified: Thu, 19 Dec 2019 23:39:41 GMT  
		Size: 128.9 MB (128912240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:9139e5151541f74a038b2172fc5c52212bbd01785ac3d2f3c96586a7fdf01ce9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.0 MB (413006807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3652ddf101ae303357779516c20848958364d96a8a77ef264da5a574d76a32`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:59:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:00:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 07:00:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:04:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:23:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:23:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22754f6fc5d5a244119c0928ebf7d851d276d7f095f07e6bf435fa7afbcab8a8`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 9.5 MB (9498197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2155e4b3456accbea4b6873247312dd288feb477ec966ed48637e031aba558`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 3.9 MB (3918728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad0ae2287846b9d91f237a798b6ae550ff58e33efb804be1ca049f9fd7a480f`  
		Last Modified: Sat, 28 Dec 2019 07:11:24 GMT  
		Size: 46.4 MB (46399839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85007ed2d2e692ae9d2693b8e9e7d47b86b28377923b5051a85c235755bfdbe`  
		Last Modified: Sat, 28 Dec 2019 07:12:26 GMT  
		Size: 195.5 MB (195523369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f204b01794ab1d4f5f363daf7ee582b1098b48ce1a0dbefa86ec5319b02ae8e4`  
		Last Modified: Sat, 28 Dec 2019 15:26:57 GMT  
		Size: 115.6 MB (115558550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:48c2253ccb471cb9ffdbb91bceffae245cceee86e04d23443a0cd0e86a23a4d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.8 MB (420789320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd1db3750013cde4e94a47ddc5130f2a253e21c99891e4e873e61d4c745f80a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:22:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:22:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:25:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:34:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:34:43 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c616dd61dc37eac19d38cdbdf732659429ae37ba0d1578100f874fe236e25125`  
		Last Modified: Fri, 22 Nov 2019 20:30:41 GMT  
		Size: 9.7 MB (9747762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df36da42882c170ff4b949c027b410428b5c0942632ed441a2f9a168a859ec0c`  
		Last Modified: Fri, 22 Nov 2019 20:30:39 GMT  
		Size: 4.1 MB (4094358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81386fcdc923e324fecbdb336d477691cc0be39e7e4e23ec733257ee50eddd57`  
		Last Modified: Fri, 22 Nov 2019 20:31:04 GMT  
		Size: 48.0 MB (48016405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6156b4a56fd4867da733a232b3da5a4312ee906bd7a09d869b3e3e026b36a5`  
		Last Modified: Fri, 22 Nov 2019 20:32:03 GMT  
		Size: 202.2 MB (202233068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd1ee4c6ce5c5845eb3bc8694b36c235eb904590d829c29e03a0beaaf54f461`  
		Last Modified: Fri, 20 Dec 2019 00:38:42 GMT  
		Size: 113.5 MB (113531421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40.0-stretch` - linux; 386

```console
$ docker pull rust@sha256:44282d01bf7fb412ef306edc631f0660feeb5827fdebe51df1aca8be4f50cdd3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478236160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c56fb4cf6e952dae9e7aeba16ef4c54fd0f4f2946a3d20a8354879aae62065b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:38:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:39:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:39:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:39:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeaedfad53e910bdc66ac7862f5f3947575aad9685d5feea1b7c59abce08f95`  
		Last Modified: Sat, 28 Dec 2019 05:47:05 GMT  
		Size: 10.8 MB (10817785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ac55b31a6a0657f064091eb17ba42f3d06984c79ad2029702e0e6abfcff01`  
		Last Modified: Sat, 28 Dec 2019 05:47:03 GMT  
		Size: 4.6 MB (4561435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e73a3cb511b1de4f269d1d6cb6912275c54f471028cbb55c137b8c6497f755`  
		Last Modified: Sat, 28 Dec 2019 05:47:23 GMT  
		Size: 51.6 MB (51595587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6b40aae89aa5be2fd05bc653e286159f74af6500ce653f8920ad8129617ca4`  
		Last Modified: Sat, 28 Dec 2019 05:48:21 GMT  
		Size: 219.9 MB (219925419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2498312f423d5ea0b74388eea648c327c989c98997819365c6fa6edb7a64a38`  
		Last Modified: Sat, 28 Dec 2019 19:42:39 GMT  
		Size: 145.2 MB (145235840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-alpine`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.40-alpine` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-alpine3.10`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.40-alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-buster`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40-buster` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-buster` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-slim`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40-slim` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-slim-buster`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-slim-stretch`

```console
$ docker pull rust@sha256:6dbd1450defc06557513c6ad040f948f25123065779ee697b611254d4d500daf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:57c6607fec3c2bfebc517cb9c13321aee87cfd84bace6f53bddbb23c15452b77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189328904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e94d78b219741c33f7ca91069f2f418bd15960e08c8ac3f31be062ac60551fbb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:37:12 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a808f9be53ad3051a0da3ba8c2600cba69684fd510f3fc12d59be3902e4e890`  
		Last Modified: Thu, 19 Dec 2019 23:40:16 GMT  
		Size: 166.8 MB (166804332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:96d44debbfd641d7873d11242e287bfba85fd21ae03e83c6eb2a0b27bf55d4fc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162934818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d1807641c5badabb356a369f86b0ec894ccbd0932211ac957dbe7a973de4e3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:23:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbdd2d07539c94add88be67e07030cdbd1863504d08306bd60b7f60d17d1d1d`  
		Last Modified: Sat, 28 Dec 2019 15:27:42 GMT  
		Size: 143.6 MB (143623231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:a1ef6c8c6d5504d56fd9f67c866ace7ad1b26f02a11a3678ad971e163f9360ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164549005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048c98f570a1ff655c5340bd5b5c6c1c90783447553197e411d6ed34e205782e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:34:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b832e63d71815acfddc8f292e3348c05ee1643280093ea87850ed9cf21a03df`  
		Last Modified: Fri, 20 Dec 2019 00:39:34 GMT  
		Size: 144.2 MB (144163246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:51de05adbfe450e2f42058374d96259cf450476b62f8fabe8fde826baaf66cb9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210290258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1e3bd06388aaad6f6f6d663b16684cd9a7aed0e8e37c6cf538bbd239d9daca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:05 GMT
ADD file:d43798bcf0e72b342c261b8585dde072d9363d19fab4b8d9f08f15db189f287b in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:39:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2cb401c016d2f9802d5ef9cf6c6dc07251e9f87757a0de0a8df318fb7f00385c`  
		Last Modified: Sat, 28 Dec 2019 04:47:36 GMT  
		Size: 23.2 MB (23152142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e7005a402b4f68ea5da5d5fbc8e568f31de042b0c63a48dea6f837fc2a4b4`  
		Last Modified: Sat, 28 Dec 2019 19:43:42 GMT  
		Size: 187.1 MB (187138116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.40-stretch`

```console
$ docker pull rust@sha256:8b678d1ce48cb057ac19cadd05162f40d80e72550153176984f604efbede66e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.40-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8799cee901791082ca011eae1eb30fd62166fee80f38284e46c28dc764f5cdf5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.3 MB (454337046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5302f1b5dabd05a5ad5f9331511d3c230d2d4963c6e168f72857636e7beabf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:15:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:36:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:07 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9577c0793430759082b98068eb2884638a34fa46ca481099e93cfc38d4ebfe`  
		Last Modified: Sat, 23 Nov 2019 00:21:35 GMT  
		Size: 214.8 MB (214841433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1501da54344da67a16aa924db62c0d8f2adda671b60360c046fa04bc9f6e6ba`  
		Last Modified: Thu, 19 Dec 2019 23:39:41 GMT  
		Size: 128.9 MB (128912240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:9139e5151541f74a038b2172fc5c52212bbd01785ac3d2f3c96586a7fdf01ce9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.0 MB (413006807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3652ddf101ae303357779516c20848958364d96a8a77ef264da5a574d76a32`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:59:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:00:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 07:00:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:04:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:23:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:23:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22754f6fc5d5a244119c0928ebf7d851d276d7f095f07e6bf435fa7afbcab8a8`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 9.5 MB (9498197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2155e4b3456accbea4b6873247312dd288feb477ec966ed48637e031aba558`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 3.9 MB (3918728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad0ae2287846b9d91f237a798b6ae550ff58e33efb804be1ca049f9fd7a480f`  
		Last Modified: Sat, 28 Dec 2019 07:11:24 GMT  
		Size: 46.4 MB (46399839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85007ed2d2e692ae9d2693b8e9e7d47b86b28377923b5051a85c235755bfdbe`  
		Last Modified: Sat, 28 Dec 2019 07:12:26 GMT  
		Size: 195.5 MB (195523369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f204b01794ab1d4f5f363daf7ee582b1098b48ce1a0dbefa86ec5319b02ae8e4`  
		Last Modified: Sat, 28 Dec 2019 15:26:57 GMT  
		Size: 115.6 MB (115558550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:48c2253ccb471cb9ffdbb91bceffae245cceee86e04d23443a0cd0e86a23a4d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.8 MB (420789320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd1db3750013cde4e94a47ddc5130f2a253e21c99891e4e873e61d4c745f80a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:22:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:22:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:25:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:34:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:34:43 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c616dd61dc37eac19d38cdbdf732659429ae37ba0d1578100f874fe236e25125`  
		Last Modified: Fri, 22 Nov 2019 20:30:41 GMT  
		Size: 9.7 MB (9747762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df36da42882c170ff4b949c027b410428b5c0942632ed441a2f9a168a859ec0c`  
		Last Modified: Fri, 22 Nov 2019 20:30:39 GMT  
		Size: 4.1 MB (4094358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81386fcdc923e324fecbdb336d477691cc0be39e7e4e23ec733257ee50eddd57`  
		Last Modified: Fri, 22 Nov 2019 20:31:04 GMT  
		Size: 48.0 MB (48016405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6156b4a56fd4867da733a232b3da5a4312ee906bd7a09d869b3e3e026b36a5`  
		Last Modified: Fri, 22 Nov 2019 20:32:03 GMT  
		Size: 202.2 MB (202233068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd1ee4c6ce5c5845eb3bc8694b36c235eb904590d829c29e03a0beaaf54f461`  
		Last Modified: Fri, 20 Dec 2019 00:38:42 GMT  
		Size: 113.5 MB (113531421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.40-stretch` - linux; 386

```console
$ docker pull rust@sha256:44282d01bf7fb412ef306edc631f0660feeb5827fdebe51df1aca8be4f50cdd3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478236160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c56fb4cf6e952dae9e7aeba16ef4c54fd0f4f2946a3d20a8354879aae62065b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:38:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:39:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:39:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:39:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeaedfad53e910bdc66ac7862f5f3947575aad9685d5feea1b7c59abce08f95`  
		Last Modified: Sat, 28 Dec 2019 05:47:05 GMT  
		Size: 10.8 MB (10817785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ac55b31a6a0657f064091eb17ba42f3d06984c79ad2029702e0e6abfcff01`  
		Last Modified: Sat, 28 Dec 2019 05:47:03 GMT  
		Size: 4.6 MB (4561435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e73a3cb511b1de4f269d1d6cb6912275c54f471028cbb55c137b8c6497f755`  
		Last Modified: Sat, 28 Dec 2019 05:47:23 GMT  
		Size: 51.6 MB (51595587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6b40aae89aa5be2fd05bc653e286159f74af6500ce653f8920ad8129617ca4`  
		Last Modified: Sat, 28 Dec 2019 05:48:21 GMT  
		Size: 219.9 MB (219925419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2498312f423d5ea0b74388eea648c327c989c98997819365c6fa6edb7a64a38`  
		Last Modified: Sat, 28 Dec 2019 19:42:39 GMT  
		Size: 145.2 MB (145235840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.10`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-buster`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-buster` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-stretch`

```console
$ docker pull rust@sha256:6dbd1450defc06557513c6ad040f948f25123065779ee697b611254d4d500daf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:57c6607fec3c2bfebc517cb9c13321aee87cfd84bace6f53bddbb23c15452b77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189328904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e94d78b219741c33f7ca91069f2f418bd15960e08c8ac3f31be062ac60551fbb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:37:12 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a808f9be53ad3051a0da3ba8c2600cba69684fd510f3fc12d59be3902e4e890`  
		Last Modified: Thu, 19 Dec 2019 23:40:16 GMT  
		Size: 166.8 MB (166804332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:96d44debbfd641d7873d11242e287bfba85fd21ae03e83c6eb2a0b27bf55d4fc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162934818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d1807641c5badabb356a369f86b0ec894ccbd0932211ac957dbe7a973de4e3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:23:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbdd2d07539c94add88be67e07030cdbd1863504d08306bd60b7f60d17d1d1d`  
		Last Modified: Sat, 28 Dec 2019 15:27:42 GMT  
		Size: 143.6 MB (143623231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:a1ef6c8c6d5504d56fd9f67c866ace7ad1b26f02a11a3678ad971e163f9360ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164549005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048c98f570a1ff655c5340bd5b5c6c1c90783447553197e411d6ed34e205782e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:34:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b832e63d71815acfddc8f292e3348c05ee1643280093ea87850ed9cf21a03df`  
		Last Modified: Fri, 20 Dec 2019 00:39:34 GMT  
		Size: 144.2 MB (144163246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:51de05adbfe450e2f42058374d96259cf450476b62f8fabe8fde826baaf66cb9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210290258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1e3bd06388aaad6f6f6d663b16684cd9a7aed0e8e37c6cf538bbd239d9daca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:05 GMT
ADD file:d43798bcf0e72b342c261b8585dde072d9363d19fab4b8d9f08f15db189f287b in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:39:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2cb401c016d2f9802d5ef9cf6c6dc07251e9f87757a0de0a8df318fb7f00385c`  
		Last Modified: Sat, 28 Dec 2019 04:47:36 GMT  
		Size: 23.2 MB (23152142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e7005a402b4f68ea5da5d5fbc8e568f31de042b0c63a48dea6f837fc2a4b4`  
		Last Modified: Sat, 28 Dec 2019 19:43:42 GMT  
		Size: 187.1 MB (187138116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-stretch`

```console
$ docker pull rust@sha256:8b678d1ce48cb057ac19cadd05162f40d80e72550153176984f604efbede66e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8799cee901791082ca011eae1eb30fd62166fee80f38284e46c28dc764f5cdf5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.3 MB (454337046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5302f1b5dabd05a5ad5f9331511d3c230d2d4963c6e168f72857636e7beabf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:15:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:36:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:07 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9577c0793430759082b98068eb2884638a34fa46ca481099e93cfc38d4ebfe`  
		Last Modified: Sat, 23 Nov 2019 00:21:35 GMT  
		Size: 214.8 MB (214841433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1501da54344da67a16aa924db62c0d8f2adda671b60360c046fa04bc9f6e6ba`  
		Last Modified: Thu, 19 Dec 2019 23:39:41 GMT  
		Size: 128.9 MB (128912240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:9139e5151541f74a038b2172fc5c52212bbd01785ac3d2f3c96586a7fdf01ce9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.0 MB (413006807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3652ddf101ae303357779516c20848958364d96a8a77ef264da5a574d76a32`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:59:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:00:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 07:00:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:04:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:23:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:23:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22754f6fc5d5a244119c0928ebf7d851d276d7f095f07e6bf435fa7afbcab8a8`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 9.5 MB (9498197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2155e4b3456accbea4b6873247312dd288feb477ec966ed48637e031aba558`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 3.9 MB (3918728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad0ae2287846b9d91f237a798b6ae550ff58e33efb804be1ca049f9fd7a480f`  
		Last Modified: Sat, 28 Dec 2019 07:11:24 GMT  
		Size: 46.4 MB (46399839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85007ed2d2e692ae9d2693b8e9e7d47b86b28377923b5051a85c235755bfdbe`  
		Last Modified: Sat, 28 Dec 2019 07:12:26 GMT  
		Size: 195.5 MB (195523369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f204b01794ab1d4f5f363daf7ee582b1098b48ce1a0dbefa86ec5319b02ae8e4`  
		Last Modified: Sat, 28 Dec 2019 15:26:57 GMT  
		Size: 115.6 MB (115558550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:48c2253ccb471cb9ffdbb91bceffae245cceee86e04d23443a0cd0e86a23a4d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.8 MB (420789320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd1db3750013cde4e94a47ddc5130f2a253e21c99891e4e873e61d4c745f80a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:22:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:22:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:25:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:34:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:34:43 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c616dd61dc37eac19d38cdbdf732659429ae37ba0d1578100f874fe236e25125`  
		Last Modified: Fri, 22 Nov 2019 20:30:41 GMT  
		Size: 9.7 MB (9747762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df36da42882c170ff4b949c027b410428b5c0942632ed441a2f9a168a859ec0c`  
		Last Modified: Fri, 22 Nov 2019 20:30:39 GMT  
		Size: 4.1 MB (4094358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81386fcdc923e324fecbdb336d477691cc0be39e7e4e23ec733257ee50eddd57`  
		Last Modified: Fri, 22 Nov 2019 20:31:04 GMT  
		Size: 48.0 MB (48016405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6156b4a56fd4867da733a232b3da5a4312ee906bd7a09d869b3e3e026b36a5`  
		Last Modified: Fri, 22 Nov 2019 20:32:03 GMT  
		Size: 202.2 MB (202233068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd1ee4c6ce5c5845eb3bc8694b36c235eb904590d829c29e03a0beaaf54f461`  
		Last Modified: Fri, 20 Dec 2019 00:38:42 GMT  
		Size: 113.5 MB (113531421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; 386

```console
$ docker pull rust@sha256:44282d01bf7fb412ef306edc631f0660feeb5827fdebe51df1aca8be4f50cdd3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478236160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c56fb4cf6e952dae9e7aeba16ef4c54fd0f4f2946a3d20a8354879aae62065b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:38:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:39:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:39:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:39:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeaedfad53e910bdc66ac7862f5f3947575aad9685d5feea1b7c59abce08f95`  
		Last Modified: Sat, 28 Dec 2019 05:47:05 GMT  
		Size: 10.8 MB (10817785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ac55b31a6a0657f064091eb17ba42f3d06984c79ad2029702e0e6abfcff01`  
		Last Modified: Sat, 28 Dec 2019 05:47:03 GMT  
		Size: 4.6 MB (4561435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e73a3cb511b1de4f269d1d6cb6912275c54f471028cbb55c137b8c6497f755`  
		Last Modified: Sat, 28 Dec 2019 05:47:23 GMT  
		Size: 51.6 MB (51595587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6b40aae89aa5be2fd05bc653e286159f74af6500ce653f8920ad8129617ca4`  
		Last Modified: Sat, 28 Dec 2019 05:48:21 GMT  
		Size: 219.9 MB (219925419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2498312f423d5ea0b74388eea648c327c989c98997819365c6fa6edb7a64a38`  
		Last Modified: Sat, 28 Dec 2019 19:42:39 GMT  
		Size: 145.2 MB (145235840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.10`

```console
$ docker pull rust@sha256:727ee417d7d59903c960fc3e33a24eff276fed201c03b4c20004ba17a8aa50b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:548700dc20e801346feb16a19ab24dbdcba7f35a8b2135b8b739b1c46cb0b7f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131087629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741bbb166a3a05a41ada837eda4bbfa1273b3646f70d7f7c17bd9fbf65b656b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:01:44 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Dec 2019 23:38:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:58 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.20.2/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "44d689d8cf49165f059cafe10a5ce49708a26b0b0641169bc0e39ad9c54930d5 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bac046ab5c04d79d04b250c2e8a820c5109feb3adb8f29ce4aafedbe33628f`  
		Last Modified: Mon, 21 Oct 2019 22:02:43 GMT  
		Size: 34.0 MB (33983607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93ba9981241b8feb11aed98dc30689fcaee3cd2c3a03dddae4bb7ec8646965`  
		Last Modified: Thu, 19 Dec 2019 23:41:45 GMT  
		Size: 94.3 MB (94316888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:buster`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:buster` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:latest`

```console
$ docker pull rust@sha256:710126921689add53fe506e0e09b30c9eea4333c516fcb76e73c9748b71e403d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:latest` - linux; amd64

```console
$ docker pull rust@sha256:5552e3511864b93c1ab9479dfa26cd2953aea9151dc51faad11d6e90b149c06c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.9 MB (440931067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9510a0988d8eca7ce1de5be9ee2ea7e089e61baf8cb2aec1401b0a5a12e245`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:37:46 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c4fb388fdfef16e8278fba2b06d46e48d152e1b40f4347c8828a04c8e2a87e`  
		Last Modified: Sat, 23 Nov 2019 00:18:22 GMT  
		Size: 192.0 MB (192044870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b40cedefe7ccaa5f34bb9b164194e396cd366f56e9acfd4da7b9460335414`  
		Last Modified: Thu, 19 Dec 2019 23:40:45 GMT  
		Size: 128.9 MB (128911998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm variant v7

```console
$ docker pull rust@sha256:8b43199e12b23fba6643472c526ce757ad9fe34e89e3485af6cb588b47745959
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393416055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719b01d71d57027ca8a7b84477c1b3a7297d2506123bb654d6ed906d009857f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:47:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:24:38 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232eea7b18919fcfc8ba4f08e15b02a8c122b9536f22a060e8cd1e8eeb2be9f`  
		Last Modified: Sat, 28 Dec 2019 07:08:17 GMT  
		Size: 168.2 MB (168242735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38bd857c3ed24b8ec3a7cdfd6252c7933d8431a1e5f61a4fe4dd973bcf56c73`  
		Last Modified: Sat, 28 Dec 2019 15:28:28 GMT  
		Size: 115.6 MB (115558525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:be1ee9d75e3cfc99fc096b92547f4dff383fa433953ef7b69d49e7bd5829c6e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.0 MB (416014283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f909636b59ed805d9048fa023cef42000026dce6f92159b948b251dd44eda15`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:25 GMT
ADD file:9f9eea5881797502bfab12007544d80607c25d2748eeeba94c931d9e83b82ca9 in / 
# Fri, 22 Nov 2019 13:41:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:12:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:12:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:16:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:36:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af4800279257e4522b03ad0d6d0aa937a2761fe0e54758127ec7fd14fc1715d0`  
		Last Modified: Fri, 22 Nov 2019 13:49:29 GMT  
		Size: 49.2 MB (49172037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae2ec46cd5af1ce11d246b5b7bea023991c857cbf131fc2b4f80a42c7abb5c`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 7.7 MB (7680704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8718b9412e0a23370b0877b007da88210a2408dd572782050dcdd233e1f19e`  
		Last Modified: Fri, 22 Nov 2019 20:27:44 GMT  
		Size: 10.0 MB (9983756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4908f8b447250af91341f8f3a1741b2c8d6432714e885746c4afd227eed1be7b`  
		Last Modified: Fri, 22 Nov 2019 20:28:07 GMT  
		Size: 52.1 MB (52079377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0fac9e6c6a4a40a22bab46b85791dc7a34b25219d893a5c2690273437194e`  
		Last Modified: Fri, 22 Nov 2019 20:29:00 GMT  
		Size: 183.6 MB (183567555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682a08a83bc70508aee1decdfa525fde8102c9343179e1f3f7b1026849103a0`  
		Last Modified: Fri, 20 Dec 2019 00:40:15 GMT  
		Size: 113.5 MB (113530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; 386

```console
$ docker pull rust@sha256:e67e6547c7cfb51044d42816c50e2f3c0ab6427158fbb6d3416cedda59867b99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0265404e7238f7bbf6d9b67acd478182425314fd467af1a13d71759011e7da1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:23:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:40:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed8ff189044a36f58bc50efb4e6be5894f2d5a2bb04f01f7e5b92d1ed2d40ed`  
		Last Modified: Sat, 28 Dec 2019 05:44:13 GMT  
		Size: 198.6 MB (198592848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a365db23765004a6abaca269aa6d850fa90258ed3f088b2fc00960a7af09e6b`  
		Last Modified: Sat, 28 Dec 2019 19:44:33 GMT  
		Size: 145.2 MB (145235309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-buster`

```console
$ docker pull rust@sha256:fe734b7fb7bbb78c3b272e3507243fa75ea6dffcf50e81a8bda9b7ee2f9d50cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:6afe324910ab55800745c84b0c307cf29fdb2426c0e01dffd9b539d53c558a30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201390356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9bf3b5eb0052e075ce684b967a094eecddaaaf0421d42cda31609aa7f4e145`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:38:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:38:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdf0b7af867c9a9c9bb7e0daba56a44f5a4d4a5d6ee84c4053f52c862a6a62`  
		Last Modified: Thu, 19 Dec 2019 23:41:21 GMT  
		Size: 174.3 MB (174297702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:bdbd8518659a52d535c37cbf2595da9ab257509788625622c1b2ffb39e1da825
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171154613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df6b56005618a313665436139edef73f0afa22cd2e807c895cb852820153628`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:25:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c059d05438cb14bc1185d40cf2e186f389b3fbff3a067ae4d09f05b3044ff9`  
		Last Modified: Sat, 28 Dec 2019 15:29:18 GMT  
		Size: 148.5 MB (148455484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2e2813c81f5254736b43b00a3fcdd6c5b773b34f825acafb67e89ed00aceab74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.6 MB (179581890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf14c2752125026f0eaadf48463c82a069d40da3f204f2e7f630a5fffd569882`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:36:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc3d3c6c299a7a4510235ba2cfdac2d0bb86d4599ef50c3a5c0f4dd4b2e9d`  
		Last Modified: Fri, 20 Dec 2019 00:41:13 GMT  
		Size: 153.7 MB (153731088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; 386

```console
$ docker pull rust@sha256:640f2c4ce13b6d0128106458ae49c2f8492cd93639b0519d46e730656e61d7cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (222959767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665f0d24924ba3f7f831a072ebc23568dd967861cf9fd74358e96f9930d01e3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:40:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:41:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4120f181d7a96ad023f4962a3e74164c74b5060bac5fde50139c2cc6d044434b`  
		Last Modified: Sat, 28 Dec 2019 19:45:50 GMT  
		Size: 195.2 MB (195212747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-stretch`

```console
$ docker pull rust@sha256:6dbd1450defc06557513c6ad040f948f25123065779ee697b611254d4d500daf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:57c6607fec3c2bfebc517cb9c13321aee87cfd84bace6f53bddbb23c15452b77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189328904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e94d78b219741c33f7ca91069f2f418bd15960e08c8ac3f31be062ac60551fbb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Thu, 19 Dec 2019 23:37:12 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a808f9be53ad3051a0da3ba8c2600cba69684fd510f3fc12d59be3902e4e890`  
		Last Modified: Thu, 19 Dec 2019 23:40:16 GMT  
		Size: 166.8 MB (166804332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:96d44debbfd641d7873d11242e287bfba85fd21ae03e83c6eb2a0b27bf55d4fc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162934818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d1807641c5badabb356a369f86b0ec894ccbd0932211ac957dbe7a973de4e3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:23:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:24:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbdd2d07539c94add88be67e07030cdbd1863504d08306bd60b7f60d17d1d1d`  
		Last Modified: Sat, 28 Dec 2019 15:27:42 GMT  
		Size: 143.6 MB (143623231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:a1ef6c8c6d5504d56fd9f67c866ace7ad1b26f02a11a3678ad971e163f9360ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164549005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048c98f570a1ff655c5340bd5b5c6c1c90783447553197e411d6ed34e205782e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 20 Dec 2019 00:34:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:36:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b832e63d71815acfddc8f292e3348c05ee1643280093ea87850ed9cf21a03df`  
		Last Modified: Fri, 20 Dec 2019 00:39:34 GMT  
		Size: 144.2 MB (144163246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:51de05adbfe450e2f42058374d96259cf450476b62f8fabe8fde826baaf66cb9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210290258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1e3bd06388aaad6f6f6d663b16684cd9a7aed0e8e37c6cf538bbd239d9daca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:05 GMT
ADD file:d43798bcf0e72b342c261b8585dde072d9363d19fab4b8d9f08f15db189f287b in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 19:39:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:40:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2cb401c016d2f9802d5ef9cf6c6dc07251e9f87757a0de0a8df318fb7f00385c`  
		Last Modified: Sat, 28 Dec 2019 04:47:36 GMT  
		Size: 23.2 MB (23152142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e7005a402b4f68ea5da5d5fbc8e568f31de042b0c63a48dea6f837fc2a4b4`  
		Last Modified: Sat, 28 Dec 2019 19:43:42 GMT  
		Size: 187.1 MB (187138116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:stretch`

```console
$ docker pull rust@sha256:8b678d1ce48cb057ac19cadd05162f40d80e72550153176984f604efbede66e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:stretch` - linux; amd64

```console
$ docker pull rust@sha256:8799cee901791082ca011eae1eb30fd62166fee80f38284e46c28dc764f5cdf5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.3 MB (454337046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5302f1b5dabd05a5ad5f9331511d3c230d2d4963c6e168f72857636e7beabf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:15:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 23:36:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Thu, 19 Dec 2019 23:37:07 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9577c0793430759082b98068eb2884638a34fa46ca481099e93cfc38d4ebfe`  
		Last Modified: Sat, 23 Nov 2019 00:21:35 GMT  
		Size: 214.8 MB (214841433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1501da54344da67a16aa924db62c0d8f2adda671b60360c046fa04bc9f6e6ba`  
		Last Modified: Thu, 19 Dec 2019 23:39:41 GMT  
		Size: 128.9 MB (128912240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:9139e5151541f74a038b2172fc5c52212bbd01785ac3d2f3c96586a7fdf01ce9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.0 MB (413006807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3652ddf101ae303357779516c20848958364d96a8a77ef264da5a574d76a32`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:59:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:00:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 07:00:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:04:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:23:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 15:23:33 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22754f6fc5d5a244119c0928ebf7d851d276d7f095f07e6bf435fa7afbcab8a8`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 9.5 MB (9498197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2155e4b3456accbea4b6873247312dd288feb477ec966ed48637e031aba558`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 3.9 MB (3918728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad0ae2287846b9d91f237a798b6ae550ff58e33efb804be1ca049f9fd7a480f`  
		Last Modified: Sat, 28 Dec 2019 07:11:24 GMT  
		Size: 46.4 MB (46399839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85007ed2d2e692ae9d2693b8e9e7d47b86b28377923b5051a85c235755bfdbe`  
		Last Modified: Sat, 28 Dec 2019 07:12:26 GMT  
		Size: 195.5 MB (195523369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f204b01794ab1d4f5f363daf7ee582b1098b48ce1a0dbefa86ec5319b02ae8e4`  
		Last Modified: Sat, 28 Dec 2019 15:26:57 GMT  
		Size: 115.6 MB (115558550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:48c2253ccb471cb9ffdbb91bceffae245cceee86e04d23443a0cd0e86a23a4d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.8 MB (420789320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd1db3750013cde4e94a47ddc5130f2a253e21c99891e4e873e61d4c745f80a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:22:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Nov 2019 20:22:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 20:25:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Dec 2019 00:34:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Fri, 20 Dec 2019 00:34:43 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c616dd61dc37eac19d38cdbdf732659429ae37ba0d1578100f874fe236e25125`  
		Last Modified: Fri, 22 Nov 2019 20:30:41 GMT  
		Size: 9.7 MB (9747762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df36da42882c170ff4b949c027b410428b5c0942632ed441a2f9a168a859ec0c`  
		Last Modified: Fri, 22 Nov 2019 20:30:39 GMT  
		Size: 4.1 MB (4094358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81386fcdc923e324fecbdb336d477691cc0be39e7e4e23ec733257ee50eddd57`  
		Last Modified: Fri, 22 Nov 2019 20:31:04 GMT  
		Size: 48.0 MB (48016405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6156b4a56fd4867da733a232b3da5a4312ee906bd7a09d869b3e3e026b36a5`  
		Last Modified: Fri, 22 Nov 2019 20:32:03 GMT  
		Size: 202.2 MB (202233068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd1ee4c6ce5c5845eb3bc8694b36c235eb904590d829c29e03a0beaaf54f461`  
		Last Modified: Fri, 20 Dec 2019 00:38:42 GMT  
		Size: 113.5 MB (113531421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; 386

```console
$ docker pull rust@sha256:44282d01bf7fb412ef306edc631f0660feeb5827fdebe51df1aca8be4f50cdd3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478236160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c56fb4cf6e952dae9e7aeba16ef4c54fd0f4f2946a3d20a8354879aae62065b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:38:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:39:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 19:39:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.40.0
# Sat, 28 Dec 2019 19:39:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='e68f193542c68ce83c449809d2cad262cc2bbb99640eb47c58fc1dc58cc30add' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='7c1c329a676e50c287d8183b88f30cd6afd0be140826a9fbbc0e3d717fab34d7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d861cc86594776414de001b96964be645c4bfa27024052704f0976dc3aed1b18' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='89f1f797dca2e5c1d75790c3c6b7be0ee473a7f4eca9663e623a41272a358da0' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.20.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeaedfad53e910bdc66ac7862f5f3947575aad9685d5feea1b7c59abce08f95`  
		Last Modified: Sat, 28 Dec 2019 05:47:05 GMT  
		Size: 10.8 MB (10817785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ac55b31a6a0657f064091eb17ba42f3d06984c79ad2029702e0e6abfcff01`  
		Last Modified: Sat, 28 Dec 2019 05:47:03 GMT  
		Size: 4.6 MB (4561435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e73a3cb511b1de4f269d1d6cb6912275c54f471028cbb55c137b8c6497f755`  
		Last Modified: Sat, 28 Dec 2019 05:47:23 GMT  
		Size: 51.6 MB (51595587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6b40aae89aa5be2fd05bc653e286159f74af6500ce653f8920ad8129617ca4`  
		Last Modified: Sat, 28 Dec 2019 05:48:21 GMT  
		Size: 219.9 MB (219925419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2498312f423d5ea0b74388eea648c327c989c98997819365c6fa6edb7a64a38`  
		Last Modified: Sat, 28 Dec 2019 19:42:39 GMT  
		Size: 145.2 MB (145235840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
