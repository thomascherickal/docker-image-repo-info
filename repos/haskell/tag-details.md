<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8-buster`](#haskell8-buster)
-	[`haskell:8-slim`](#haskell8-slim)
-	[`haskell:8-slim-buster`](#haskell8-slim-buster)
-	[`haskell:8.10`](#haskell810)
-	[`haskell:8.10-buster`](#haskell810-buster)
-	[`haskell:8.10-slim`](#haskell810-slim)
-	[`haskell:8.10-slim-buster`](#haskell810-slim-buster)
-	[`haskell:8.10.7`](#haskell8107)
-	[`haskell:8.10.7-buster`](#haskell8107-buster)
-	[`haskell:8.10.7-slim`](#haskell8107-slim)
-	[`haskell:8.10.7-slim-buster`](#haskell8107-slim-buster)
-	[`haskell:9`](#haskell9)
-	[`haskell:9-buster`](#haskell9-buster)
-	[`haskell:9-slim`](#haskell9-slim)
-	[`haskell:9-slim-buster`](#haskell9-slim-buster)
-	[`haskell:9.0`](#haskell90)
-	[`haskell:9.0-buster`](#haskell90-buster)
-	[`haskell:9.0-slim`](#haskell90-slim)
-	[`haskell:9.0-slim-buster`](#haskell90-slim-buster)
-	[`haskell:9.0.2`](#haskell902)
-	[`haskell:9.0.2-buster`](#haskell902-buster)
-	[`haskell:9.0.2-slim`](#haskell902-slim)
-	[`haskell:9.0.2-slim-buster`](#haskell902-slim-buster)
-	[`haskell:9.2`](#haskell92)
-	[`haskell:9.2-buster`](#haskell92-buster)
-	[`haskell:9.2-slim`](#haskell92-slim)
-	[`haskell:9.2-slim-buster`](#haskell92-slim-buster)
-	[`haskell:9.2.4`](#haskell924)
-	[`haskell:9.2.4-buster`](#haskell924-buster)
-	[`haskell:9.2.4-slim`](#haskell924-slim)
-	[`haskell:9.2.4-slim-buster`](#haskell924-slim-buster)
-	[`haskell:9.4`](#haskell94)
-	[`haskell:9.4-buster`](#haskell94-buster)
-	[`haskell:9.4-slim`](#haskell94-slim)
-	[`haskell:9.4-slim-buster`](#haskell94-slim-buster)
-	[`haskell:9.4.2`](#haskell942)
-	[`haskell:9.4.2-buster`](#haskell942-buster)
-	[`haskell:9.4.2-slim`](#haskell942-slim)
-	[`haskell:9.4.2-slim-buster`](#haskell942-slim-buster)
-	[`haskell:buster`](#haskellbuster)
-	[`haskell:latest`](#haskelllatest)
-	[`haskell:slim`](#haskellslim)
-	[`haskell:slim-buster`](#haskellslim-buster)

## `haskell:8`

```console
$ docker pull haskell@sha256:f2b6ea003e068966b508c9041689a7eb0b322612b833d8ebdf3a9ac6120a4bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:c38804b87bd64dce802c1a3fc5bd1021069b820b27612ac2d1e3e0396f5ad49c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **665.5 MB (665468351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b2034825283d068503ee8abb402c4b14fb875aa4840c905026489cf2febe5a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC=8.10.7
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:55:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:55:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:55:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadeb09b8b0f49bcb4542d49ca7ee9a88063f9fa832c7c7f457202fab88206f0`  
		Last Modified: Wed, 05 Oct 2022 04:06:18 GMT  
		Size: 330.5 MB (330502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b3065f3cc38fad1d0c7f0720f38c4263ce1718789c6cc6225dff0c518a45eed0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **852.3 MB (852336034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e3807e6626f48d38b9c5cb6eb6e9c57598ab46adddd44d590cfedaa602f18`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:06:18 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:06:35 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:06:35 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c03dfb85742031572baafa6aa2487d1a7b142ebade1f4cd16c17086f592f1`  
		Last Modified: Tue, 25 Oct 2022 10:17:05 GMT  
		Size: 490.3 MB (490327790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:f2b6ea003e068966b508c9041689a7eb0b322612b833d8ebdf3a9ac6120a4bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:c38804b87bd64dce802c1a3fc5bd1021069b820b27612ac2d1e3e0396f5ad49c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **665.5 MB (665468351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b2034825283d068503ee8abb402c4b14fb875aa4840c905026489cf2febe5a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC=8.10.7
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:55:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:55:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:55:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadeb09b8b0f49bcb4542d49ca7ee9a88063f9fa832c7c7f457202fab88206f0`  
		Last Modified: Wed, 05 Oct 2022 04:06:18 GMT  
		Size: 330.5 MB (330502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b3065f3cc38fad1d0c7f0720f38c4263ce1718789c6cc6225dff0c518a45eed0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **852.3 MB (852336034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e3807e6626f48d38b9c5cb6eb6e9c57598ab46adddd44d590cfedaa602f18`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:06:18 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:06:35 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:06:35 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c03dfb85742031572baafa6aa2487d1a7b142ebade1f4cd16c17086f592f1`  
		Last Modified: Tue, 25 Oct 2022 10:17:05 GMT  
		Size: 490.3 MB (490327790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-slim`

```console
$ docker pull haskell@sha256:d6c07d7003e1e315252afd47faf52ee6698b03af0bc3bcb2ff89b7d0d9c49747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8-slim` - linux; amd64

```console
$ docker pull haskell@sha256:8a6861a75a3fa680023cc25293614797fe0fbdf4bb5b0f8cf20095a77e17b9cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357487494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3cd3300170006e5864ba234263fb15be2066ab58db66beafd918d5f09646dea`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:47:42 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:47:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:47:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8352024ecb2e6e3c19027cce7540a7a764cd7783788a5ea06a70d861c05eb9ca`  
		Last Modified: Tue, 25 Oct 2022 03:52:22 GMT  
		Size: 214.5 MB (214525968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:a0e75900b9c23be5c446ae4e995b873e2725d113f3b3b524199c3cb14f68331f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **511.0 MB (510979637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a07bf86d8b104ec449a3f41e52c60754ac533b82dce0afeaf32388da3aa6fd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:08:05 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:08:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:08:17 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eecaefc43274ca1adf2a07e4ecc2ac713db2114bb64877f4c09a61410c7ad5`  
		Last Modified: Tue, 25 Oct 2022 10:18:24 GMT  
		Size: 324.8 MB (324808217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-slim-buster`

```console
$ docker pull haskell@sha256:d6c07d7003e1e315252afd47faf52ee6698b03af0bc3bcb2ff89b7d0d9c49747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:8a6861a75a3fa680023cc25293614797fe0fbdf4bb5b0f8cf20095a77e17b9cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357487494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3cd3300170006e5864ba234263fb15be2066ab58db66beafd918d5f09646dea`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:47:42 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:47:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:47:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8352024ecb2e6e3c19027cce7540a7a764cd7783788a5ea06a70d861c05eb9ca`  
		Last Modified: Tue, 25 Oct 2022 03:52:22 GMT  
		Size: 214.5 MB (214525968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:a0e75900b9c23be5c446ae4e995b873e2725d113f3b3b524199c3cb14f68331f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **511.0 MB (510979637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a07bf86d8b104ec449a3f41e52c60754ac533b82dce0afeaf32388da3aa6fd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:08:05 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:08:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:08:17 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eecaefc43274ca1adf2a07e4ecc2ac713db2114bb64877f4c09a61410c7ad5`  
		Last Modified: Tue, 25 Oct 2022 10:18:24 GMT  
		Size: 324.8 MB (324808217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:f2b6ea003e068966b508c9041689a7eb0b322612b833d8ebdf3a9ac6120a4bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:c38804b87bd64dce802c1a3fc5bd1021069b820b27612ac2d1e3e0396f5ad49c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **665.5 MB (665468351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b2034825283d068503ee8abb402c4b14fb875aa4840c905026489cf2febe5a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC=8.10.7
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:55:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:55:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:55:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadeb09b8b0f49bcb4542d49ca7ee9a88063f9fa832c7c7f457202fab88206f0`  
		Last Modified: Wed, 05 Oct 2022 04:06:18 GMT  
		Size: 330.5 MB (330502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b3065f3cc38fad1d0c7f0720f38c4263ce1718789c6cc6225dff0c518a45eed0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **852.3 MB (852336034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e3807e6626f48d38b9c5cb6eb6e9c57598ab46adddd44d590cfedaa602f18`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:06:18 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:06:35 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:06:35 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c03dfb85742031572baafa6aa2487d1a7b142ebade1f4cd16c17086f592f1`  
		Last Modified: Tue, 25 Oct 2022 10:17:05 GMT  
		Size: 490.3 MB (490327790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:f2b6ea003e068966b508c9041689a7eb0b322612b833d8ebdf3a9ac6120a4bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:c38804b87bd64dce802c1a3fc5bd1021069b820b27612ac2d1e3e0396f5ad49c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **665.5 MB (665468351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b2034825283d068503ee8abb402c4b14fb875aa4840c905026489cf2febe5a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC=8.10.7
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:55:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:55:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:55:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadeb09b8b0f49bcb4542d49ca7ee9a88063f9fa832c7c7f457202fab88206f0`  
		Last Modified: Wed, 05 Oct 2022 04:06:18 GMT  
		Size: 330.5 MB (330502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b3065f3cc38fad1d0c7f0720f38c4263ce1718789c6cc6225dff0c518a45eed0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **852.3 MB (852336034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e3807e6626f48d38b9c5cb6eb6e9c57598ab46adddd44d590cfedaa602f18`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:06:18 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:06:35 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:06:35 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c03dfb85742031572baafa6aa2487d1a7b142ebade1f4cd16c17086f592f1`  
		Last Modified: Tue, 25 Oct 2022 10:17:05 GMT  
		Size: 490.3 MB (490327790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-slim`

```console
$ docker pull haskell@sha256:d6c07d7003e1e315252afd47faf52ee6698b03af0bc3bcb2ff89b7d0d9c49747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10-slim` - linux; amd64

```console
$ docker pull haskell@sha256:8a6861a75a3fa680023cc25293614797fe0fbdf4bb5b0f8cf20095a77e17b9cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357487494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3cd3300170006e5864ba234263fb15be2066ab58db66beafd918d5f09646dea`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:47:42 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:47:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:47:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8352024ecb2e6e3c19027cce7540a7a764cd7783788a5ea06a70d861c05eb9ca`  
		Last Modified: Tue, 25 Oct 2022 03:52:22 GMT  
		Size: 214.5 MB (214525968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:a0e75900b9c23be5c446ae4e995b873e2725d113f3b3b524199c3cb14f68331f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **511.0 MB (510979637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a07bf86d8b104ec449a3f41e52c60754ac533b82dce0afeaf32388da3aa6fd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:08:05 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:08:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:08:17 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eecaefc43274ca1adf2a07e4ecc2ac713db2114bb64877f4c09a61410c7ad5`  
		Last Modified: Tue, 25 Oct 2022 10:18:24 GMT  
		Size: 324.8 MB (324808217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-slim-buster`

```console
$ docker pull haskell@sha256:d6c07d7003e1e315252afd47faf52ee6698b03af0bc3bcb2ff89b7d0d9c49747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:8a6861a75a3fa680023cc25293614797fe0fbdf4bb5b0f8cf20095a77e17b9cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357487494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3cd3300170006e5864ba234263fb15be2066ab58db66beafd918d5f09646dea`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:47:42 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:47:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:47:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8352024ecb2e6e3c19027cce7540a7a764cd7783788a5ea06a70d861c05eb9ca`  
		Last Modified: Tue, 25 Oct 2022 03:52:22 GMT  
		Size: 214.5 MB (214525968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:a0e75900b9c23be5c446ae4e995b873e2725d113f3b3b524199c3cb14f68331f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **511.0 MB (510979637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a07bf86d8b104ec449a3f41e52c60754ac533b82dce0afeaf32388da3aa6fd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:08:05 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:08:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:08:17 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eecaefc43274ca1adf2a07e4ecc2ac713db2114bb64877f4c09a61410c7ad5`  
		Last Modified: Tue, 25 Oct 2022 10:18:24 GMT  
		Size: 324.8 MB (324808217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7`

```console
$ docker pull haskell@sha256:f2b6ea003e068966b508c9041689a7eb0b322612b833d8ebdf3a9ac6120a4bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10.7` - linux; amd64

```console
$ docker pull haskell@sha256:c38804b87bd64dce802c1a3fc5bd1021069b820b27612ac2d1e3e0396f5ad49c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **665.5 MB (665468351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b2034825283d068503ee8abb402c4b14fb875aa4840c905026489cf2febe5a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC=8.10.7
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:55:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:55:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:55:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadeb09b8b0f49bcb4542d49ca7ee9a88063f9fa832c7c7f457202fab88206f0`  
		Last Modified: Wed, 05 Oct 2022 04:06:18 GMT  
		Size: 330.5 MB (330502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10.7` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b3065f3cc38fad1d0c7f0720f38c4263ce1718789c6cc6225dff0c518a45eed0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **852.3 MB (852336034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e3807e6626f48d38b9c5cb6eb6e9c57598ab46adddd44d590cfedaa602f18`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:06:18 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:06:35 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:06:35 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c03dfb85742031572baafa6aa2487d1a7b142ebade1f4cd16c17086f592f1`  
		Last Modified: Tue, 25 Oct 2022 10:17:05 GMT  
		Size: 490.3 MB (490327790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7-buster`

```console
$ docker pull haskell@sha256:f2b6ea003e068966b508c9041689a7eb0b322612b833d8ebdf3a9ac6120a4bab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10.7-buster` - linux; amd64

```console
$ docker pull haskell@sha256:c38804b87bd64dce802c1a3fc5bd1021069b820b27612ac2d1e3e0396f5ad49c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **665.5 MB (665468351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b2034825283d068503ee8abb402c4b14fb875aa4840c905026489cf2febe5a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC=8.10.7
# Wed, 05 Oct 2022 03:54:38 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:55:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:55:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:55:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadeb09b8b0f49bcb4542d49ca7ee9a88063f9fa832c7c7f457202fab88206f0`  
		Last Modified: Wed, 05 Oct 2022 04:06:18 GMT  
		Size: 330.5 MB (330502492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10.7-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b3065f3cc38fad1d0c7f0720f38c4263ce1718789c6cc6225dff0c518a45eed0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **852.3 MB (852336034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e3807e6626f48d38b9c5cb6eb6e9c57598ab46adddd44d590cfedaa602f18`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:04:53 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:06:18 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:06:35 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:06:35 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c03dfb85742031572baafa6aa2487d1a7b142ebade1f4cd16c17086f592f1`  
		Last Modified: Tue, 25 Oct 2022 10:17:05 GMT  
		Size: 490.3 MB (490327790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7-slim`

```console
$ docker pull haskell@sha256:d6c07d7003e1e315252afd47faf52ee6698b03af0bc3bcb2ff89b7d0d9c49747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10.7-slim` - linux; amd64

```console
$ docker pull haskell@sha256:8a6861a75a3fa680023cc25293614797fe0fbdf4bb5b0f8cf20095a77e17b9cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357487494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3cd3300170006e5864ba234263fb15be2066ab58db66beafd918d5f09646dea`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:47:42 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:47:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:47:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8352024ecb2e6e3c19027cce7540a7a764cd7783788a5ea06a70d861c05eb9ca`  
		Last Modified: Tue, 25 Oct 2022 03:52:22 GMT  
		Size: 214.5 MB (214525968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10.7-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:a0e75900b9c23be5c446ae4e995b873e2725d113f3b3b524199c3cb14f68331f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **511.0 MB (510979637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a07bf86d8b104ec449a3f41e52c60754ac533b82dce0afeaf32388da3aa6fd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:08:05 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:08:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:08:17 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eecaefc43274ca1adf2a07e4ecc2ac713db2114bb64877f4c09a61410c7ad5`  
		Last Modified: Tue, 25 Oct 2022 10:18:24 GMT  
		Size: 324.8 MB (324808217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7-slim-buster`

```console
$ docker pull haskell@sha256:d6c07d7003e1e315252afd47faf52ee6698b03af0bc3bcb2ff89b7d0d9c49747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:8.10.7-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:8a6861a75a3fa680023cc25293614797fe0fbdf4bb5b0f8cf20095a77e17b9cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357487494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3cd3300170006e5864ba234263fb15be2066ab58db66beafd918d5f09646dea`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 03:46:47 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:47:42 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:47:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:47:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8352024ecb2e6e3c19027cce7540a7a764cd7783788a5ea06a70d861c05eb9ca`  
		Last Modified: Tue, 25 Oct 2022 03:52:22 GMT  
		Size: 214.5 MB (214525968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:8.10.7-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:a0e75900b9c23be5c446ae4e995b873e2725d113f3b3b524199c3cb14f68331f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **511.0 MB (510979637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a07bf86d8b104ec449a3f41e52c60754ac533b82dce0afeaf32388da3aa6fd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC=8.10.7
# Tue, 25 Oct 2022 10:06:45 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:08:05 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fad2417f9b295233bf8ade79c0e6140896359e87be46cb61cd1d35863d9d0e55';             ;;         'x86_64')             GHC_SHA256='a13719bca87a0d3ac0c7d4157a4e60887009a7f1a8dbe95c4759ec413e086d30';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:08:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:08:17 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eecaefc43274ca1adf2a07e4ecc2ac713db2114bb64877f4c09a61410c7ad5`  
		Last Modified: Tue, 25 Oct 2022 10:18:24 GMT  
		Size: 324.8 MB (324808217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-slim`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-slim` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-slim-buster`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:02457ac7f2660fa79c29c496ab4b11d2d594e524bd2655c3dc52505fef0bd8ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:40cf77fa68b369620a411718cf5e8c696823f219ea761b32053af858df81fab3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **661.4 MB (661376458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe8ba109c9d876bacc9d7b1ae9068f609e7e651ed71a7106dfd358cc5465275`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC=9.0.2
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:53:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:53:19 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:53:19 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935b3da6b264848fc8820ee45993e5987621b6646113b00de6f01b47d23a9973`  
		Last Modified: Wed, 05 Oct 2022 04:03:56 GMT  
		Size: 326.4 MB (326410599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2c7d415ac36e2da55f5ca8d3fd2f32d76f5f633a08481339c318d1837ace7c7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.0 MB (592990273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135b4f48e655f4f0f43d098975349688c2b1fc97b828dee3bb9673acc85d0a37`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:03:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:03:32 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:03:32 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f70a3061536a36ed93ce33dd62532a14049fad017dfd6a236c5e161573b2d7`  
		Last Modified: Tue, 25 Oct 2022 10:14:31 GMT  
		Size: 231.0 MB (230982029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:02457ac7f2660fa79c29c496ab4b11d2d594e524bd2655c3dc52505fef0bd8ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:40cf77fa68b369620a411718cf5e8c696823f219ea761b32053af858df81fab3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **661.4 MB (661376458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe8ba109c9d876bacc9d7b1ae9068f609e7e651ed71a7106dfd358cc5465275`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC=9.0.2
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:53:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:53:19 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:53:19 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935b3da6b264848fc8820ee45993e5987621b6646113b00de6f01b47d23a9973`  
		Last Modified: Wed, 05 Oct 2022 04:03:56 GMT  
		Size: 326.4 MB (326410599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2c7d415ac36e2da55f5ca8d3fd2f32d76f5f633a08481339c318d1837ace7c7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.0 MB (592990273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135b4f48e655f4f0f43d098975349688c2b1fc97b828dee3bb9673acc85d0a37`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:03:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:03:32 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:03:32 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f70a3061536a36ed93ce33dd62532a14049fad017dfd6a236c5e161573b2d7`  
		Last Modified: Tue, 25 Oct 2022 10:14:31 GMT  
		Size: 231.0 MB (230982029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-slim`

```console
$ docker pull haskell@sha256:2efb088762292c2fd2f0eb270e8e39862224d5579567d3a3c54789265f6a00e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0-slim` - linux; amd64

```console
$ docker pull haskell@sha256:e5655b869c70ac7b8dcada1bede04bfa9734a0c66278aac4230efb7d04eadddc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.9 MB (352934993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c7a0b60db2bfbf177fb5be29ee505fe4b2cb7c2893114bcdb6298266f25293`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:46:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:46:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:46:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ee4f9b4c0ef475b257f1edd840e890000bda79137fdad146063cfa2ebb9a8e`  
		Last Modified: Tue, 25 Oct 2022 03:51:22 GMT  
		Size: 210.0 MB (209973467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:33e78607b6342c0e1e4aef3390c4e3bedf80d475e87bbff12206c9842666ac88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.2 MB (417150618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1614b19af3d33f1683e74266d6cbc95ec7bf526bcbd65466218911fb9a39446b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:04:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:04:42 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:04:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514e3311e2e3a00730cd832c3181c25b20c00085d13593175daf187d82314b1f`  
		Last Modified: Tue, 25 Oct 2022 10:15:26 GMT  
		Size: 231.0 MB (230979198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-slim-buster`

```console
$ docker pull haskell@sha256:2efb088762292c2fd2f0eb270e8e39862224d5579567d3a3c54789265f6a00e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e5655b869c70ac7b8dcada1bede04bfa9734a0c66278aac4230efb7d04eadddc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.9 MB (352934993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c7a0b60db2bfbf177fb5be29ee505fe4b2cb7c2893114bcdb6298266f25293`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:46:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:46:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:46:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ee4f9b4c0ef475b257f1edd840e890000bda79137fdad146063cfa2ebb9a8e`  
		Last Modified: Tue, 25 Oct 2022 03:51:22 GMT  
		Size: 210.0 MB (209973467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:33e78607b6342c0e1e4aef3390c4e3bedf80d475e87bbff12206c9842666ac88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.2 MB (417150618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1614b19af3d33f1683e74266d6cbc95ec7bf526bcbd65466218911fb9a39446b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:04:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:04:42 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:04:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514e3311e2e3a00730cd832c3181c25b20c00085d13593175daf187d82314b1f`  
		Last Modified: Tue, 25 Oct 2022 10:15:26 GMT  
		Size: 231.0 MB (230979198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2`

```console
$ docker pull haskell@sha256:02457ac7f2660fa79c29c496ab4b11d2d594e524bd2655c3dc52505fef0bd8ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2` - linux; amd64

```console
$ docker pull haskell@sha256:40cf77fa68b369620a411718cf5e8c696823f219ea761b32053af858df81fab3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **661.4 MB (661376458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe8ba109c9d876bacc9d7b1ae9068f609e7e651ed71a7106dfd358cc5465275`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC=9.0.2
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:53:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:53:19 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:53:19 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935b3da6b264848fc8820ee45993e5987621b6646113b00de6f01b47d23a9973`  
		Last Modified: Wed, 05 Oct 2022 04:03:56 GMT  
		Size: 326.4 MB (326410599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2c7d415ac36e2da55f5ca8d3fd2f32d76f5f633a08481339c318d1837ace7c7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.0 MB (592990273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135b4f48e655f4f0f43d098975349688c2b1fc97b828dee3bb9673acc85d0a37`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:03:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:03:32 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:03:32 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f70a3061536a36ed93ce33dd62532a14049fad017dfd6a236c5e161573b2d7`  
		Last Modified: Tue, 25 Oct 2022 10:14:31 GMT  
		Size: 231.0 MB (230982029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2-buster`

```console
$ docker pull haskell@sha256:02457ac7f2660fa79c29c496ab4b11d2d594e524bd2655c3dc52505fef0bd8ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:40cf77fa68b369620a411718cf5e8c696823f219ea761b32053af858df81fab3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **661.4 MB (661376458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe8ba109c9d876bacc9d7b1ae9068f609e7e651ed71a7106dfd358cc5465275`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_VERSION=12
# Wed, 05 Oct 2022 03:52:06 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 05 Oct 2022 03:52:07 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC=9.0.2
# Wed, 05 Oct 2022 03:52:07 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:53:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:53:19 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:53:19 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935b3da6b264848fc8820ee45993e5987621b6646113b00de6f01b47d23a9973`  
		Last Modified: Wed, 05 Oct 2022 04:03:56 GMT  
		Size: 326.4 MB (326410599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2c7d415ac36e2da55f5ca8d3fd2f32d76f5f633a08481339c318d1837ace7c7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.0 MB (592990273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135b4f48e655f4f0f43d098975349688c2b1fc97b828dee3bb9673acc85d0a37`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:02:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:02:43 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:02:44 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:03:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:03:32 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:03:32 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf760079bb62077d6d50b2100e600d4b8e71f72cc8afd2b08c49969c0bf864`  
		Last Modified: Tue, 25 Oct 2022 10:13:56 GMT  
		Size: 45.9 MB (45889114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f70a3061536a36ed93ce33dd62532a14049fad017dfd6a236c5e161573b2d7`  
		Last Modified: Tue, 25 Oct 2022 10:14:31 GMT  
		Size: 231.0 MB (230982029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2-slim`

```console
$ docker pull haskell@sha256:2efb088762292c2fd2f0eb270e8e39862224d5579567d3a3c54789265f6a00e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2-slim` - linux; amd64

```console
$ docker pull haskell@sha256:e5655b869c70ac7b8dcada1bede04bfa9734a0c66278aac4230efb7d04eadddc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.9 MB (352934993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c7a0b60db2bfbf177fb5be29ee505fe4b2cb7c2893114bcdb6298266f25293`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:46:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:46:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:46:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ee4f9b4c0ef475b257f1edd840e890000bda79137fdad146063cfa2ebb9a8e`  
		Last Modified: Tue, 25 Oct 2022 03:51:22 GMT  
		Size: 210.0 MB (209973467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:33e78607b6342c0e1e4aef3390c4e3bedf80d475e87bbff12206c9842666ac88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.2 MB (417150618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1614b19af3d33f1683e74266d6cbc95ec7bf526bcbd65466218911fb9a39446b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:04:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:04:42 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:04:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514e3311e2e3a00730cd832c3181c25b20c00085d13593175daf187d82314b1f`  
		Last Modified: Tue, 25 Oct 2022 10:15:26 GMT  
		Size: 231.0 MB (230979198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2-slim-buster`

```console
$ docker pull haskell@sha256:2efb088762292c2fd2f0eb270e8e39862224d5579567d3a3c54789265f6a00e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e5655b869c70ac7b8dcada1bede04bfa9734a0c66278aac4230efb7d04eadddc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.9 MB (352934993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c7a0b60db2bfbf177fb5be29ee505fe4b2cb7c2893114bcdb6298266f25293`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 03:45:35 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 03:45:36 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 03:45:36 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:46:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:46:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:46:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ee4f9b4c0ef475b257f1edd840e890000bda79137fdad146063cfa2ebb9a8e`  
		Last Modified: Tue, 25 Oct 2022 03:51:22 GMT  
		Size: 210.0 MB (209973467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:33e78607b6342c0e1e4aef3390c4e3bedf80d475e87bbff12206c9842666ac88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.2 MB (417150618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1614b19af3d33f1683e74266d6cbc95ec7bf526bcbd65466218911fb9a39446b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_VERSION=12
# Tue, 25 Oct 2022 10:03:44 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Tue, 25 Oct 2022 10:03:51 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC=9.0.2
# Tue, 25 Oct 2022 10:03:52 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:04:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:04:42 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:04:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e66ec371761a7ee5ec3566fe8976defc2ae5c662ded58847660d1aca8aa87`  
		Last Modified: Tue, 25 Oct 2022 10:14:52 GMT  
		Size: 59.8 MB (59835699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514e3311e2e3a00730cd832c3181c25b20c00085d13593175daf187d82314b1f`  
		Last Modified: Tue, 25 Oct 2022 10:15:26 GMT  
		Size: 231.0 MB (230979198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2`

```console
$ docker pull haskell@sha256:84c5925f32ee73b17ddc5e8716cca1619d226c49e67bdb836e2ac58cf094eb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2` - linux; amd64

```console
$ docker pull haskell@sha256:43993e3f9c77f81f09055275d8c60b73f7aba0775625521730ec398f50631abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.4 MB (676438886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a9439a00db41c55826367b900460334f5988355a6904fdd105ab7daf30bfbd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC=9.2.4
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:50:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:50:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:50:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea930d4a7b91b81299ee2203ac6236dfbb42be87e64edb51852651cb88198645`  
		Last Modified: Wed, 05 Oct 2022 04:01:34 GMT  
		Size: 341.5 MB (341473027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:13423d60f9fbca2f588924aa222b6dd446dd5483be6dadc9cf0c03b7231bed91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.4 MB (722449595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46026b63f6b307cd1519b09c036f40a413afc2c2379c3edb063a2cf4cd847a07`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:00:26 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:00:41 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:00:41 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d5029213254e2eb8d9f9b3070028ead2772d61c8f70d3c49d26d8619b47287`  
		Last Modified: Tue, 25 Oct 2022 10:12:34 GMT  
		Size: 406.3 MB (406330465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2-buster`

```console
$ docker pull haskell@sha256:84c5925f32ee73b17ddc5e8716cca1619d226c49e67bdb836e2ac58cf094eb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:43993e3f9c77f81f09055275d8c60b73f7aba0775625521730ec398f50631abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.4 MB (676438886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a9439a00db41c55826367b900460334f5988355a6904fdd105ab7daf30bfbd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC=9.2.4
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:50:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:50:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:50:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea930d4a7b91b81299ee2203ac6236dfbb42be87e64edb51852651cb88198645`  
		Last Modified: Wed, 05 Oct 2022 04:01:34 GMT  
		Size: 341.5 MB (341473027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:13423d60f9fbca2f588924aa222b6dd446dd5483be6dadc9cf0c03b7231bed91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.4 MB (722449595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46026b63f6b307cd1519b09c036f40a413afc2c2379c3edb063a2cf4cd847a07`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:00:26 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:00:41 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:00:41 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d5029213254e2eb8d9f9b3070028ead2772d61c8f70d3c49d26d8619b47287`  
		Last Modified: Tue, 25 Oct 2022 10:12:34 GMT  
		Size: 406.3 MB (406330465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2-slim`

```console
$ docker pull haskell@sha256:e0796bd135d6975f149bc9580b489b3748c34246087df9a88d52dfe5c93c0c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2-slim` - linux; amd64

```console
$ docker pull haskell@sha256:063884d367ba3cf8d5d05eff5d9cfbbc669f57ad5c557f2e76ca046e91aa3608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362346598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9139182e9259367279fe4e0e96be958620db67e95cf113a82fb6bf5beb3ec7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:45:14 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:45:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:45:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a567a67fa6c6bd227d5d9013773d7d695b2a7c7733ce8ac611a66f6ce95739`  
		Last Modified: Tue, 25 Oct 2022 03:50:23 GMT  
		Size: 219.4 MB (219385072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:d629f6988e2203d8f570b3e5c04399f7bab361cc65afbeb7f63ee3e77a704a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.7 MB (387678958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967b306dd11dc762dd8144bcca9b9090f921394673095e9463fef4a273303345`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:02:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:02:23 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:02:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652de59a0b9dc78b474f14512e8720feb52544fd51848a9453ffe29fa3c23800`  
		Last Modified: Tue, 25 Oct 2022 10:13:37 GMT  
		Size: 261.3 MB (261343237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2-slim-buster`

```console
$ docker pull haskell@sha256:e0796bd135d6975f149bc9580b489b3748c34246087df9a88d52dfe5c93c0c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:063884d367ba3cf8d5d05eff5d9cfbbc669f57ad5c557f2e76ca046e91aa3608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362346598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9139182e9259367279fe4e0e96be958620db67e95cf113a82fb6bf5beb3ec7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:45:14 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:45:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:45:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a567a67fa6c6bd227d5d9013773d7d695b2a7c7733ce8ac611a66f6ce95739`  
		Last Modified: Tue, 25 Oct 2022 03:50:23 GMT  
		Size: 219.4 MB (219385072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:d629f6988e2203d8f570b3e5c04399f7bab361cc65afbeb7f63ee3e77a704a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.7 MB (387678958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967b306dd11dc762dd8144bcca9b9090f921394673095e9463fef4a273303345`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:02:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:02:23 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:02:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652de59a0b9dc78b474f14512e8720feb52544fd51848a9453ffe29fa3c23800`  
		Last Modified: Tue, 25 Oct 2022 10:13:37 GMT  
		Size: 261.3 MB (261343237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.4`

```console
$ docker pull haskell@sha256:84c5925f32ee73b17ddc5e8716cca1619d226c49e67bdb836e2ac58cf094eb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.4` - linux; amd64

```console
$ docker pull haskell@sha256:43993e3f9c77f81f09055275d8c60b73f7aba0775625521730ec398f50631abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.4 MB (676438886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a9439a00db41c55826367b900460334f5988355a6904fdd105ab7daf30bfbd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC=9.2.4
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:50:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:50:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:50:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea930d4a7b91b81299ee2203ac6236dfbb42be87e64edb51852651cb88198645`  
		Last Modified: Wed, 05 Oct 2022 04:01:34 GMT  
		Size: 341.5 MB (341473027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.4` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:13423d60f9fbca2f588924aa222b6dd446dd5483be6dadc9cf0c03b7231bed91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.4 MB (722449595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46026b63f6b307cd1519b09c036f40a413afc2c2379c3edb063a2cf4cd847a07`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:00:26 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:00:41 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:00:41 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d5029213254e2eb8d9f9b3070028ead2772d61c8f70d3c49d26d8619b47287`  
		Last Modified: Tue, 25 Oct 2022 10:12:34 GMT  
		Size: 406.3 MB (406330465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.4-buster`

```console
$ docker pull haskell@sha256:84c5925f32ee73b17ddc5e8716cca1619d226c49e67bdb836e2ac58cf094eb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:43993e3f9c77f81f09055275d8c60b73f7aba0775625521730ec398f50631abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.4 MB (676438886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a9439a00db41c55826367b900460334f5988355a6904fdd105ab7daf30bfbd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC=9.2.4
# Wed, 05 Oct 2022 03:49:33 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 05 Oct 2022 03:50:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:50:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:50:47 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea930d4a7b91b81299ee2203ac6236dfbb42be87e64edb51852651cb88198645`  
		Last Modified: Wed, 05 Oct 2022 04:01:34 GMT  
		Size: 341.5 MB (341473027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.4-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:13423d60f9fbca2f588924aa222b6dd446dd5483be6dadc9cf0c03b7231bed91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.4 MB (722449595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46026b63f6b307cd1519b09c036f40a413afc2c2379c3edb063a2cf4cd847a07`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 09:59:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:00:26 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:00:41 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:00:41 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d5029213254e2eb8d9f9b3070028ead2772d61c8f70d3c49d26d8619b47287`  
		Last Modified: Tue, 25 Oct 2022 10:12:34 GMT  
		Size: 406.3 MB (406330465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.4-slim`

```console
$ docker pull haskell@sha256:e0796bd135d6975f149bc9580b489b3748c34246087df9a88d52dfe5c93c0c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.4-slim` - linux; amd64

```console
$ docker pull haskell@sha256:063884d367ba3cf8d5d05eff5d9cfbbc669f57ad5c557f2e76ca046e91aa3608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362346598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9139182e9259367279fe4e0e96be958620db67e95cf113a82fb6bf5beb3ec7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:45:14 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:45:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:45:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a567a67fa6c6bd227d5d9013773d7d695b2a7c7733ce8ac611a66f6ce95739`  
		Last Modified: Tue, 25 Oct 2022 03:50:23 GMT  
		Size: 219.4 MB (219385072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.4-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:d629f6988e2203d8f570b3e5c04399f7bab361cc65afbeb7f63ee3e77a704a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.7 MB (387678958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967b306dd11dc762dd8144bcca9b9090f921394673095e9463fef4a273303345`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:02:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:02:23 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:02:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652de59a0b9dc78b474f14512e8720feb52544fd51848a9453ffe29fa3c23800`  
		Last Modified: Tue, 25 Oct 2022 10:13:37 GMT  
		Size: 261.3 MB (261343237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.4-slim-buster`

```console
$ docker pull haskell@sha256:e0796bd135d6975f149bc9580b489b3748c34246087df9a88d52dfe5c93c0c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.4-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:063884d367ba3cf8d5d05eff5d9cfbbc669f57ad5c557f2e76ca046e91aa3608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362346598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9139182e9259367279fe4e0e96be958620db67e95cf113a82fb6bf5beb3ec7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 03:44:10 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 03:45:14 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:45:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:45:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a567a67fa6c6bd227d5d9013773d7d695b2a7c7733ce8ac611a66f6ce95739`  
		Last Modified: Tue, 25 Oct 2022 03:50:23 GMT  
		Size: 219.4 MB (219385072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.4-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:d629f6988e2203d8f570b3e5c04399f7bab361cc65afbeb7f63ee3e77a704a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.7 MB (387678958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967b306dd11dc762dd8144bcca9b9090f921394673095e9463fef4a273303345`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC=9.2.4
# Tue, 25 Oct 2022 10:00:57 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 25 Oct 2022 10:02:12 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.4 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='fc7dbc6bae36ea5ac30b7e9a263b7e5be3b45b0eb3e893ad0bc2c950a61f14ec';             ;;         'x86_64')             GHC_SHA256='a77a91a39d9b0167124b7e97648b2b52973ae0978cb259e0d44f0752a75037cb';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 10:02:23 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:02:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652de59a0b9dc78b474f14512e8720feb52544fd51848a9453ffe29fa3c23800`  
		Last Modified: Tue, 25 Oct 2022 10:13:37 GMT  
		Size: 261.3 MB (261343237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4-buster`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4-slim`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4-slim` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4-slim-buster`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.2`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.2` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.2` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.2-buster`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.2-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.2-slim`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.2-slim` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.2-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.2-slim-buster`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.2-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:f6d08b5778de0f775231078138303c03e83e40d7b4eee984c9778c98adaa4525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:3bece736a4a050c057526e2423c0b84016f2839f30446c609990c79f539a5f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **647.0 MB (647040354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b17a051e0e0d9239fecc4da213f6a8d3d7883c94500f73920da35914d38b31f`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:58:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:47 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:45:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK=2.9.1
# Wed, 05 Oct 2022 03:45:52 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 05 Oct 2022 03:45:55 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 05 Oct 2022 03:45:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 05 Oct 2022 03:45:58 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC=9.4.2
# Wed, 05 Oct 2022 03:45:58 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 05 Oct 2022 03:47:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 05 Oct 2022 03:47:25 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 03:47:25 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0ae5ed3318e8db87d129f9c2652dddc78c89f223625a345ec1b7b84149a882`  
		Last Modified: Wed, 05 Oct 2022 01:21:16 GMT  
		Size: 192.5 MB (192505482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1bb9f818bf66aaf600378632f8c782171dc09667eb89707fa97d9fe566d8bb`  
		Last Modified: Wed, 05 Oct 2022 03:57:53 GMT  
		Size: 513.1 KB (513093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9639ec02a6be34997231b07e7c9dc6b37cc06a7c642eaad4f017c0e61a89896`  
		Last Modified: Wed, 05 Oct 2022 03:57:55 GMT  
		Size: 14.0 MB (13967937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b731c4ded79852e1d1f504a2a526573ec3c7b68aff524e4c31bd9734b08c5887`  
		Last Modified: Wed, 05 Oct 2022 03:57:54 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be54dc637df7b9ecf0a052bbde8fb732d5128f642169c8564b5c3851c8bcb09`  
		Last Modified: Wed, 05 Oct 2022 03:58:53 GMT  
		Size: 312.1 MB (312074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:latest` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:3e8a2a5e2299d87b662cb8a6eebe8967279dadf98a44b45efb6fa21bd5df3372
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **676.5 MB (676543410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2e50d65ac91857be66b9fda4ab0797784d09e4a2218bb5215693946bf1896bd`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:00:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:01:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:55:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:55:38 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:55:39 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:55:39 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:55:41 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:55:41 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:56:52 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:57:05 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:57:05 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5909a8b8cad57ca90fe69eaa8b350c722b820753f9caaa1f528f2337a71f38`  
		Last Modified: Tue, 25 Oct 2022 08:31:26 GMT  
		Size: 7.7 MB (7726424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a633475baeae1eb12baa14cc54f130d1e37ea520470ee16bb2dd23d779d08b4b`  
		Last Modified: Tue, 25 Oct 2022 08:31:25 GMT  
		Size: 10.0 MB (10003562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f22a2b8ddcb8bb5d37d3cd14e13998148d107dc8eb1d7c57c3220c1915fd9d1`  
		Last Modified: Tue, 25 Oct 2022 08:31:41 GMT  
		Size: 52.2 MB (52172864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985dd0945ed8d7e2674a61279668f6edeac4dc80a4a6a517fd01736884e37951`  
		Last Modified: Tue, 25 Oct 2022 08:32:08 GMT  
		Size: 184.1 MB (184093104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c73e04aae360e99ac5f7e6a1bd405dd295c9bb16ee8108b4baacc3716c08e`  
		Last Modified: Tue, 25 Oct 2022 10:09:08 GMT  
		Size: 516.7 KB (516712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b29557f7e2c465efe2ad1f471bf376ea9c1018777ba285620b68e7f505168`  
		Last Modified: Tue, 25 Oct 2022 10:09:09 GMT  
		Size: 12.4 MB (12373184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6723fb85a3cef4017f258af7c9ef46d306a4af61e24e91245e421248700389e`  
		Last Modified: Tue, 25 Oct 2022 10:10:05 GMT  
		Size: 360.4 MB (360424280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:slim`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:slim` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:slim-buster`

```console
$ docker pull haskell@sha256:c9a7b8c3d71d70280c7e0f2e753c856259b6aa4c9d2abe391ce1442ed1cc1418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:abe90883e6917c4aa6c68ab437f4f507db369297180109e594b3492969661a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336497659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cb79a4afd0ccc6a0a14e591fdfb23d68b3650348d292de72499a653bb00dec`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:42:14 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 03:42:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 03:42:37 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 03:42:42 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 03:42:42 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 03:42:43 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 03:42:45 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 03:42:45 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 03:44:00 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 03:44:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 03:44:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06176de7775b02532735290157976b793f7715c74c4688bfa9143f086ca8e030`  
		Last Modified: Tue, 25 Oct 2022 03:48:51 GMT  
		Size: 94.0 MB (94014372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470fbde626421901d68c4058b8d1d3f7ca9ab2a2b9959bdb3add63fc27a9da98`  
		Last Modified: Tue, 25 Oct 2022 03:48:40 GMT  
		Size: 14.0 MB (13967942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8892229b17c90795aaff94544a33968b58a766942ec4804811b4f6091065ec`  
		Last Modified: Tue, 25 Oct 2022 03:48:39 GMT  
		Size: 7.8 MB (7838380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa2db0a9a54cc162577228d87d95650e12f61137d215c55b684f4a8b2df735`  
		Last Modified: Tue, 25 Oct 2022 03:49:14 GMT  
		Size: 193.5 MB (193536133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:2f0d6896431197669a7dfad8ea25e9d0e8be9e85e0b978993bc58eee225dd75a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343319444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01efa91cb8d0f0dd3e50c8c8cacdc7f62942c49ba5b9a4449ff7451fc5347ac`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:57:12 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 09:57:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK=2.9.1
# Tue, 25 Oct 2022 09:57:31 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 25 Oct 2022 09:57:31 GMT
# ARGS: STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='0581cebe880b8ed47556ee73d8bbb9d602b5b82e38f89f6aa53acaec37e7760d';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Tue, 25 Oct 2022 09:57:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Tue, 25 Oct 2022 09:57:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC=9.4.2
# Tue, 25 Oct 2022 09:57:34 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 25 Oct 2022 09:58:44 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.9.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='ea075c54143dde37ea50cd085af61abb1fcfce8913deac298adc328bbb349464';             ;;         'x86_64')             GHC_SHA256='5bf34ef70a2b824d45e525f09690c76707b7f01698962e425e8fd78b94ea9174';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Tue, 25 Oct 2022 09:58:51 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:58:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b193d847424f93ccb5e65a2ff7a71e511c74bb0cd7a9723075c4ca88d4246`  
		Last Modified: Tue, 25 Oct 2022 10:10:42 GMT  
		Size: 88.0 MB (88047643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb453d87c95cba7cdd247771f7646cfba9dd5170a1089785b5325eae681699df`  
		Last Modified: Tue, 25 Oct 2022 10:10:33 GMT  
		Size: 12.4 MB (12373193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe80083d796fde274de5be9c8a3984ff1609405605d17221f1a180e190ea0a1`  
		Last Modified: Tue, 25 Oct 2022 10:11:04 GMT  
		Size: 217.0 MB (216983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
