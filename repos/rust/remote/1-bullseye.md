## `rust:1-bullseye`

```console
$ docker pull rust@sha256:d3283bad172c19e319e19125bc4d2e22a495dfef2796d9ae0968b0504b568ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:b9331b83517a41d3c0d5dceb4ac83f3fc2c1b6d9781d8284d783ba04a7efd9ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **513.6 MB (513624854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a86e6dc91a5bb7c47aaae91a2fa79eacc3a0ee7d4e468734ab19203e2419717e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:31:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 09:06:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 04 Jul 2023 09:06:53 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa786a946ae67fa18e07eaf82fefee1777449f7db1a8fea5abec1aadbe99e2ef`  
		Last Modified: Tue, 04 Jul 2023 03:52:45 GMT  
		Size: 54.6 MB (54585046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f8721393bc605f2b915d80eb2ad6d5219db374f36bbd1fee99b99174a0a4ca`  
		Last Modified: Tue, 04 Jul 2023 03:53:17 GMT  
		Size: 196.9 MB (196850887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304750e295b5d88534a737e75e676ca82e2accf2ca1a42d4c70bfa10a917362e`  
		Last Modified: Tue, 04 Jul 2023 09:10:32 GMT  
		Size: 191.4 MB (191373294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:13a909bb8db5ec71354d2494204a35b4db665d681eb8cd5244806c48d6642d05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.3 MB (493286972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3226ed3d692a07afa94101b939153b223b517b62be1d1f5eb37a6662798c9ffa`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:56:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:57:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 14:16:35 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 13 Jun 2023 14:16:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38186e5e226995fff4cc17f64810ad935c484e3a9ac1011f1e1dd7e61981e00`  
		Last Modified: Tue, 13 Jun 2023 05:03:59 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c8a738a3f9fa6d18fee05626fa2589151c6bb8ec6839f944ec47292b813314`  
		Last Modified: Tue, 13 Jun 2023 05:04:28 GMT  
		Size: 167.3 MB (167330026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24592ab76f7b59fe2e29b347519d95c082ff63f710f2a72b717f97dad752769b`  
		Last Modified: Tue, 13 Jun 2023 14:22:08 GMT  
		Size: 210.5 MB (210514538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0be891692284e51d8bf5546cfe422c50e80497df23e5a8ab0a699b58c462077e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.7 MB (557699200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f9b1c643172c1aefbdf0c1068915456145ed798809fabb856cc3f98bfed8ed`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:03:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 13:54:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 13 Jun 2023 13:54:50 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b90602383b5196ae0f8744277182f671de6f12c55664a9f36b274ab9266b5cc`  
		Last Modified: Tue, 13 Jun 2023 03:08:47 GMT  
		Size: 54.7 MB (54676037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f590ba6f72d8516eac5d7bc3811a5cd0eda704dad8f42e6cb00e86955f01231`  
		Last Modified: Tue, 13 Jun 2023 03:09:12 GMT  
		Size: 189.8 MB (189768557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e574e8693deed50a64b58aaf40f8441b235723943591b0258c14300b4c13789c`  
		Last Modified: Tue, 13 Jun 2023 13:58:56 GMT  
		Size: 243.8 MB (243803907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; 386

```console
$ docker pull rust@sha256:dc31853bad9bd8667277c7c64d4a6d9157a599ed2e32fb1398cc97304d3727de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **520.9 MB (520916374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09c271d7feb1a0ef80ce290b8b944e822cffc51872f96da0509d747db8d1baa`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:04:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:05:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:06:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:38:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 13 Jun 2023 20:39:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f5dde02e53ba41cbb376df97a5a106dcdacfee9b317fa635acdef0e92431e5`  
		Last Modified: Tue, 13 Jun 2023 01:12:41 GMT  
		Size: 16.3 MB (16263400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cdbadabe8bfab344a3144f3f66656501fb58a09d1d76acaba00818ee00d3aa`  
		Last Modified: Tue, 13 Jun 2023 01:13:02 GMT  
		Size: 55.9 MB (55922892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d890f973ce59f79c776bbdf39dab089bc74d94d765e990b7a7166de3bd61ac83`  
		Last Modified: Tue, 13 Jun 2023 01:13:47 GMT  
		Size: 199.8 MB (199766168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2d2c1a87da055cb2d3e55940bfcace9110bbd4a47c807cf6e681fd80702f6c`  
		Last Modified: Tue, 13 Jun 2023 20:41:30 GMT  
		Size: 192.9 MB (192923249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
