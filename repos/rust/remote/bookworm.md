## `rust:bookworm`

```console
$ docker pull rust@sha256:dfd1f510e48104c662cca8682dbfb06db279da854f2817a3c692aafcbf090988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:bookworm` - linux; amd64

```console
$ docker pull rust@sha256:999b052355eb874d4f196daeaf62b3d754b913cad8fc434d7e88edce494ea35e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.1 MB (522125802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7af5c2fc46d50f5a9bad8977c661212264bce251593a4165d5358d8a62152cc0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:29:51 GMT
ADD file:98917c081507795b8ce084d09f5df75e959c5365882d73ca7a52da226c93fdcf in / 
# Thu, 23 Mar 2023 01:29:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:59:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 05:59:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 05:59:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:01:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 01:30:12 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Fri, 24 Mar 2023 01:30:26 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c15c60aea1a8c926f00ec7713f9ae1fcd349591095bddcc01ee5a6027b8a3998`  
		Last Modified: Thu, 23 Mar 2023 01:33:26 GMT  
		Size: 49.3 MB (49278011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7a10c25fd2bd2e34fb5e4a59e626d6bbc6f8fda13a14dd73e631b3c91c2e3c`  
		Last Modified: Thu, 23 Mar 2023 06:07:02 GMT  
		Size: 9.1 MB (9081481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d04ad2d6622983195ee4a7f6a29b48e631f0f4722d7d32ca1a3920924f91e`  
		Last Modified: Thu, 23 Mar 2023 06:07:02 GMT  
		Size: 11.4 MB (11405655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053a14ef866632b1dc597565e4bfda17dac048c000873ef340a5eda753918dd2`  
		Last Modified: Thu, 23 Mar 2023 06:07:18 GMT  
		Size: 64.1 MB (64096758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f46df857c8d969e17b7bf0708bd43e6bf89b366b216dba35d3059324f155659`  
		Last Modified: Thu, 23 Mar 2023 06:07:52 GMT  
		Size: 210.9 MB (210921427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc727c8fa751f0ab6724d3ffce24320036d7126b7aa7687bafa223938d3561`  
		Last Modified: Fri, 24 Mar 2023 01:35:31 GMT  
		Size: 177.3 MB (177342470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bookworm` - linux; arm variant v7

```console
$ docker pull rust@sha256:4d8d96ef1dbae51c964273a034538ae298a8ac60be5b766b86b3ad8202f5f4dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.8 MB (509772940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769cde6b75d3f6b7028dcb9e98d03b2b2022298373dbb0437f2af2c845d42e51`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 22:34:58 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Thu, 23 Mar 2023 22:35:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3318c652dc50d1377b04d3c6d10a08df4155179df516ddbb594b1e7df246`  
		Last Modified: Thu, 23 Mar 2023 12:44:21 GMT  
		Size: 59.2 MB (59244953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23277d44a430ca9622032448c2da0203a6bd89b1246d243611b93d52ed2fa502`  
		Last Modified: Thu, 23 Mar 2023 12:44:51 GMT  
		Size: 174.9 MB (174948416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7d6ec3503cd0cdcf24d8672e1f9e0f654023c45e43b00240e4e614bf3f2cc4`  
		Last Modified: Thu, 23 Mar 2023 22:40:14 GMT  
		Size: 210.8 MB (210834221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bookworm` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:35928d2ffc5857b4258258826dbe71a902b8e3e20422222edc6c4bb8b2fcacb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.1 MB (579143666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:840da30a93dd2fff46aa678098403ef6c81d4e48914be9eaba2a2000c7a40f8a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:48 GMT
ADD file:fc54d0a42f70d91c654d7ac03aa3d437fad192d9f4fd701e214da74c18630636 in / 
# Thu, 23 Mar 2023 00:44:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:09:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:09:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:10:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 22:35:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Thu, 23 Mar 2023 22:35:50 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b813e5ae6de73806a605f44184f1b7d14569e88447b46841154803d1dd1eb646`  
		Last Modified: Thu, 23 Mar 2023 00:47:13 GMT  
		Size: 49.3 MB (49328280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699d2c7ce01662547528b6d61e036191dbfe660303bab6f430344734845b3291`  
		Last Modified: Thu, 23 Mar 2023 07:16:16 GMT  
		Size: 8.9 MB (8914423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f716da59b3846ca60aabeb709b6096ee3b11de955af29949f2e1ea56c6e43331`  
		Last Modified: Thu, 23 Mar 2023 07:16:16 GMT  
		Size: 11.4 MB (11371822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea922ed2e8c56f9c3f7e34565ff8c487367b1790564bc0012bba00eeae27c0b`  
		Last Modified: Thu, 23 Mar 2023 07:16:31 GMT  
		Size: 64.0 MB (63960489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeabfbfc233a69cb3a8d2d241ee8caa8df9fdbce5896eaf8c85b14e13458cd84`  
		Last Modified: Thu, 23 Mar 2023 07:16:58 GMT  
		Size: 202.4 MB (202353408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12593ddd81a259d59379f3d1e34ad0bc676e8456e83dab04626152dc0f1b7372`  
		Last Modified: Thu, 23 Mar 2023 22:41:14 GMT  
		Size: 243.2 MB (243215244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bookworm` - linux; 386

```console
$ docker pull rust@sha256:cdec63a780232197d5a0f5e628f567bd58d9c6154f54a63d399cdd29e63662c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539623966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883081ae1785927c03eab749ecc9e134e8f827f77e86c65c54fd4dcc8b98fc03`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:38:46 GMT
ADD file:a8b128db07f7f5c47ccd2afe2595fdf9b31844beff2d07ae2ea0e204e2aef4c9 in / 
# Thu, 23 Mar 2023 00:38:47 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:42:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:45:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 21:09:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.0
# Thu, 23 Mar 2023 21:10:13 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4dc30e65d953c72fa1dd5a25980f7eeea620434c102211fdb72a04706c06dd96`  
		Last Modified: Thu, 23 Mar 2023 00:42:07 GMT  
		Size: 50.3 MB (50323933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4e857b25978a7d4a42bbc134bf1ee209791d8f3fff94cb3745d9753472886a`  
		Last Modified: Thu, 23 Mar 2023 13:51:54 GMT  
		Size: 9.3 MB (9261870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845682110df86e268754e9c3ecfa5297b566a487052aaf7766ae3e9bb0cfe5bb`  
		Last Modified: Thu, 23 Mar 2023 13:51:54 GMT  
		Size: 11.8 MB (11809101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344955241ef85247f437d61d4cb8379bff720c035818b5d81495909e577561fe`  
		Last Modified: Thu, 23 Mar 2023 13:52:16 GMT  
		Size: 66.0 MB (65955359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83d29f4ffabb43db0e6af5373532c55e664f263df93209d6ca4a6e2858f33b8`  
		Last Modified: Thu, 23 Mar 2023 13:53:01 GMT  
		Size: 209.9 MB (209857051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c7438aabd87505ee9b7022be2969099c29485c45baac5786dc43da59f74b99`  
		Last Modified: Thu, 23 Mar 2023 21:15:58 GMT  
		Size: 192.4 MB (192416652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
