<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

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
-	[`haskell:9.2.8`](#haskell928)
-	[`haskell:9.2.8-buster`](#haskell928-buster)
-	[`haskell:9.2.8-slim`](#haskell928-slim)
-	[`haskell:9.2.8-slim-buster`](#haskell928-slim-buster)
-	[`haskell:9.4`](#haskell94)
-	[`haskell:9.4-buster`](#haskell94-buster)
-	[`haskell:9.4-slim`](#haskell94-slim)
-	[`haskell:9.4-slim-buster`](#haskell94-slim-buster)
-	[`haskell:9.4.7`](#haskell947)
-	[`haskell:9.4.7-buster`](#haskell947-buster)
-	[`haskell:9.4.7-slim`](#haskell947-slim)
-	[`haskell:9.4.7-slim-buster`](#haskell947-slim-buster)
-	[`haskell:9.6`](#haskell96)
-	[`haskell:9.6-buster`](#haskell96-buster)
-	[`haskell:9.6-slim`](#haskell96-slim)
-	[`haskell:9.6-slim-buster`](#haskell96-slim-buster)
-	[`haskell:9.6.2`](#haskell962)
-	[`haskell:9.6.2-buster`](#haskell962-buster)
-	[`haskell:9.6.2-slim`](#haskell962-slim)
-	[`haskell:9.6.2-slim-buster`](#haskell962-slim-buster)
-	[`haskell:buster`](#haskellbuster)
-	[`haskell:latest`](#haskelllatest)
-	[`haskell:slim`](#haskellslim)
-	[`haskell:slim-buster`](#haskellslim-buster)

## `haskell:9`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-slim`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-slim` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-slim-buster`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:20b922970e54e8acd41b5ea9dd045c5923864d3c7303b373fae22e09b91d78ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:f096e25d6459776ddaad0d111a1a7d9566ef14dc5afc722f8662c37f9b60b4a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.1 MB (717128692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fa6fecf7ce8b92e3b1fe60e1780bbec26ef627884f7e087b9eb44371ce347`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:57:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:58:49 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:58:55 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:58:55 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dbc0d8d0b83ea04ccf63c79c2728315dd8f87ec93f1f06a148c399305a588f`  
		Last Modified: Thu, 07 Sep 2023 04:09:56 GMT  
		Size: 381.6 MB (381553689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:ff3c3e8d58a88cdac8b67446c64d848bb92ab4ea6907ecdac54386a1da2a2e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.8 MB (641756627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369cc585a57092112a549ce0013bf152b61bc2dd4199c839525cae3e29a278e0`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_VERSION=12
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 16 Aug 2023 03:19:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 16 Aug 2023 03:19:47 GMT
ARG GHC=9.0.2
# Wed, 16 Aug 2023 03:19:48 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:20:30 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:20:39 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:20:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a117389239dae9962011fc2e482658063b67866a48b2447422ef0d394338535`  
		Last Modified: Wed, 16 Aug 2023 03:27:33 GMT  
		Size: 45.9 MB (45889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8790b9c1ab987289c9457d782c922abe41e22db24e423ec1fa7c84f1ae78652`  
		Last Modified: Wed, 16 Aug 2023 03:28:13 GMT  
		Size: 263.3 MB (263322581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:20b922970e54e8acd41b5ea9dd045c5923864d3c7303b373fae22e09b91d78ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f096e25d6459776ddaad0d111a1a7d9566ef14dc5afc722f8662c37f9b60b4a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.1 MB (717128692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fa6fecf7ce8b92e3b1fe60e1780bbec26ef627884f7e087b9eb44371ce347`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:57:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:58:49 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:58:55 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:58:55 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dbc0d8d0b83ea04ccf63c79c2728315dd8f87ec93f1f06a148c399305a588f`  
		Last Modified: Thu, 07 Sep 2023 04:09:56 GMT  
		Size: 381.6 MB (381553689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:ff3c3e8d58a88cdac8b67446c64d848bb92ab4ea6907ecdac54386a1da2a2e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.8 MB (641756627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369cc585a57092112a549ce0013bf152b61bc2dd4199c839525cae3e29a278e0`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_VERSION=12
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 16 Aug 2023 03:19:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 16 Aug 2023 03:19:47 GMT
ARG GHC=9.0.2
# Wed, 16 Aug 2023 03:19:48 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:20:30 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:20:39 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:20:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a117389239dae9962011fc2e482658063b67866a48b2447422ef0d394338535`  
		Last Modified: Wed, 16 Aug 2023 03:27:33 GMT  
		Size: 45.9 MB (45889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8790b9c1ab987289c9457d782c922abe41e22db24e423ec1fa7c84f1ae78652`  
		Last Modified: Wed, 16 Aug 2023 03:28:13 GMT  
		Size: 263.3 MB (263322581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-slim`

```console
$ docker pull haskell@sha256:0e0aab6f28f5cb2410e94fb3a4e6b47c2e58d56cffd53e4b120be5f853a8cfbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0-slim` - linux; amd64

```console
$ docker pull haskell@sha256:da51a320975ce0162abe8def0aa3222ebe3101ac7a0cbcfbcfcc890aa58d7c9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.6 MB (409555495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd4906d738d25de1ff63c84b59d45a72f003918033441bc018b33da07c6a648`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:59:01 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 04:00:10 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 04:00:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 04:00:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf667912063b8438dc79633cdfa6423e0c77e4344e6da6d42a6bb491d40cc5a`  
		Last Modified: Thu, 07 Sep 2023 04:11:02 GMT  
		Size: 265.1 MB (265124876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:05680efc411b6182a07a335cebf98eafa4d4ad1d2f374fd9eaaa9a852d75d1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466779278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b734e8f18b28b90f668220af3ec3e183fd1dde0f04e9f40c5b076c844bbfc7d2`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 01:45:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:46:17 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:46:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:46:27 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc87f06e906a7d93291eb13515b48330f9f556cc34e5564b35d5ddc0af400d`  
		Last Modified: Thu, 07 Sep 2023 01:50:07 GMT  
		Size: 59.8 MB (59836019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0822880af66ee51ffa9a1eb170a089632f0701bdae270a4b3461a316366b4a0`  
		Last Modified: Thu, 07 Sep 2023 01:50:43 GMT  
		Size: 263.3 MB (263318378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-slim-buster`

```console
$ docker pull haskell@sha256:0e0aab6f28f5cb2410e94fb3a4e6b47c2e58d56cffd53e4b120be5f853a8cfbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:da51a320975ce0162abe8def0aa3222ebe3101ac7a0cbcfbcfcc890aa58d7c9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.6 MB (409555495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd4906d738d25de1ff63c84b59d45a72f003918033441bc018b33da07c6a648`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:59:01 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 04:00:10 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 04:00:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 04:00:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf667912063b8438dc79633cdfa6423e0c77e4344e6da6d42a6bb491d40cc5a`  
		Last Modified: Thu, 07 Sep 2023 04:11:02 GMT  
		Size: 265.1 MB (265124876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:05680efc411b6182a07a335cebf98eafa4d4ad1d2f374fd9eaaa9a852d75d1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466779278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b734e8f18b28b90f668220af3ec3e183fd1dde0f04e9f40c5b076c844bbfc7d2`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 01:45:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:46:17 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:46:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:46:27 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc87f06e906a7d93291eb13515b48330f9f556cc34e5564b35d5ddc0af400d`  
		Last Modified: Thu, 07 Sep 2023 01:50:07 GMT  
		Size: 59.8 MB (59836019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0822880af66ee51ffa9a1eb170a089632f0701bdae270a4b3461a316366b4a0`  
		Last Modified: Thu, 07 Sep 2023 01:50:43 GMT  
		Size: 263.3 MB (263318378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2`

```console
$ docker pull haskell@sha256:20b922970e54e8acd41b5ea9dd045c5923864d3c7303b373fae22e09b91d78ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2` - linux; amd64

```console
$ docker pull haskell@sha256:f096e25d6459776ddaad0d111a1a7d9566ef14dc5afc722f8662c37f9b60b4a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.1 MB (717128692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fa6fecf7ce8b92e3b1fe60e1780bbec26ef627884f7e087b9eb44371ce347`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:57:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:58:49 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:58:55 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:58:55 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dbc0d8d0b83ea04ccf63c79c2728315dd8f87ec93f1f06a148c399305a588f`  
		Last Modified: Thu, 07 Sep 2023 04:09:56 GMT  
		Size: 381.6 MB (381553689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:ff3c3e8d58a88cdac8b67446c64d848bb92ab4ea6907ecdac54386a1da2a2e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.8 MB (641756627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369cc585a57092112a549ce0013bf152b61bc2dd4199c839525cae3e29a278e0`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_VERSION=12
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 16 Aug 2023 03:19:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 16 Aug 2023 03:19:47 GMT
ARG GHC=9.0.2
# Wed, 16 Aug 2023 03:19:48 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:20:30 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:20:39 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:20:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a117389239dae9962011fc2e482658063b67866a48b2447422ef0d394338535`  
		Last Modified: Wed, 16 Aug 2023 03:27:33 GMT  
		Size: 45.9 MB (45889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8790b9c1ab987289c9457d782c922abe41e22db24e423ec1fa7c84f1ae78652`  
		Last Modified: Wed, 16 Aug 2023 03:28:13 GMT  
		Size: 263.3 MB (263322581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2-buster`

```console
$ docker pull haskell@sha256:20b922970e54e8acd41b5ea9dd045c5923864d3c7303b373fae22e09b91d78ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f096e25d6459776ddaad0d111a1a7d9566ef14dc5afc722f8662c37f9b60b4a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.1 MB (717128692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626fa6fecf7ce8b92e3b1fe60e1780bbec26ef627884f7e087b9eb44371ce347`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:57:36 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:57:37 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:57:37 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:58:49 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:58:55 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:58:55 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dbc0d8d0b83ea04ccf63c79c2728315dd8f87ec93f1f06a148c399305a588f`  
		Last Modified: Thu, 07 Sep 2023 04:09:56 GMT  
		Size: 381.6 MB (381553689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:ff3c3e8d58a88cdac8b67446c64d848bb92ab4ea6907ecdac54386a1da2a2e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.8 MB (641756627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369cc585a57092112a549ce0013bf152b61bc2dd4199c839525cae3e29a278e0`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_VERSION=12
# Wed, 16 Aug 2023 03:19:38 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Wed, 16 Aug 2023 03:19:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Wed, 16 Aug 2023 03:19:47 GMT
ARG GHC=9.0.2
# Wed, 16 Aug 2023 03:19:48 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:20:30 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:20:39 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:20:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a117389239dae9962011fc2e482658063b67866a48b2447422ef0d394338535`  
		Last Modified: Wed, 16 Aug 2023 03:27:33 GMT  
		Size: 45.9 MB (45889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8790b9c1ab987289c9457d782c922abe41e22db24e423ec1fa7c84f1ae78652`  
		Last Modified: Wed, 16 Aug 2023 03:28:13 GMT  
		Size: 263.3 MB (263322581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2-slim`

```console
$ docker pull haskell@sha256:0e0aab6f28f5cb2410e94fb3a4e6b47c2e58d56cffd53e4b120be5f853a8cfbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2-slim` - linux; amd64

```console
$ docker pull haskell@sha256:da51a320975ce0162abe8def0aa3222ebe3101ac7a0cbcfbcfcc890aa58d7c9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.6 MB (409555495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd4906d738d25de1ff63c84b59d45a72f003918033441bc018b33da07c6a648`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:59:01 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 04:00:10 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 04:00:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 04:00:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf667912063b8438dc79633cdfa6423e0c77e4344e6da6d42a6bb491d40cc5a`  
		Last Modified: Thu, 07 Sep 2023 04:11:02 GMT  
		Size: 265.1 MB (265124876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:05680efc411b6182a07a335cebf98eafa4d4ad1d2f374fd9eaaa9a852d75d1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466779278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b734e8f18b28b90f668220af3ec3e183fd1dde0f04e9f40c5b076c844bbfc7d2`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 01:45:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:46:17 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:46:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:46:27 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc87f06e906a7d93291eb13515b48330f9f556cc34e5564b35d5ddc0af400d`  
		Last Modified: Thu, 07 Sep 2023 01:50:07 GMT  
		Size: 59.8 MB (59836019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0822880af66ee51ffa9a1eb170a089632f0701bdae270a4b3461a316366b4a0`  
		Last Modified: Thu, 07 Sep 2023 01:50:43 GMT  
		Size: 263.3 MB (263318378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.2-slim-buster`

```console
$ docker pull haskell@sha256:0e0aab6f28f5cb2410e94fb3a4e6b47c2e58d56cffd53e4b120be5f853a8cfbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.0.2-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:da51a320975ce0162abe8def0aa3222ebe3101ac7a0cbcfbcfcc890aa58d7c9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.6 MB (409555495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd4906d738d25de1ff63c84b59d45a72f003918033441bc018b33da07c6a648`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 03:59:00 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 03:59:01 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 03:59:01 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 04:00:10 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 04:00:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 04:00:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf667912063b8438dc79633cdfa6423e0c77e4344e6da6d42a6bb491d40cc5a`  
		Last Modified: Thu, 07 Sep 2023 04:11:02 GMT  
		Size: 265.1 MB (265124876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.0.2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:05680efc411b6182a07a335cebf98eafa4d4ad1d2f374fd9eaaa9a852d75d1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466779278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b734e8f18b28b90f668220af3ec3e183fd1dde0f04e9f40c5b076c844bbfc7d2`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_VERSION=12
# Thu, 07 Sep 2023 01:45:23 GMT
ARG LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421
# Thu, 07 Sep 2023 01:45:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     if [ "$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" = "aarch64" ]; then         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         mkdir -p /usr/local/share/keyrings/;         gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$LLVM_KEY";         gpg --batch --armor --export "$LLVM_KEY" > /usr/local/share/keyrings/apt.llvm.org.gpg.asc;         echo "deb [ signed-by=/usr/local/share/keyrings/apt.llvm.org.gpg.asc ] http://apt.llvm.org/buster/ llvm-toolchain-buster-$LLVM_VERSION main" > /etc/apt/sources.list.d/llvm.list;         apt-get update;         apt-get install -y --no-install-recommends llvm-$LLVM_VERSION;         gpgconf --kill all;         rm -rf "$GNUPGHOME" /var/lib/apt/lists/*;     fi
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC=9.0.2
# Thu, 07 Sep 2023 01:45:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:46:17 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.0.2 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 LLVM_KEY=6084F3CF814B57C1CF12EFD515CF4D18AF4F7421 LLVM_VERSION=12 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='cb016344c70a872738a24af60bd15d3b18749087b9905c1b3f1b1549dc01f46d';             ;;         'x86_64')             GHC_SHA256='5d0b9414b10cfb918453bcd01c5ea7a1824fe95948b08498d6780f20ba247afc';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:46:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:46:27 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc87f06e906a7d93291eb13515b48330f9f556cc34e5564b35d5ddc0af400d`  
		Last Modified: Thu, 07 Sep 2023 01:50:07 GMT  
		Size: 59.8 MB (59836019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0822880af66ee51ffa9a1eb170a089632f0701bdae270a4b3461a316366b4a0`  
		Last Modified: Thu, 07 Sep 2023 01:50:43 GMT  
		Size: 263.3 MB (263318378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2`

```console
$ docker pull haskell@sha256:21f26d54e749b7773c6a6df1ef27ec9a5310a22028c4e858f3a60251f4fac941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2` - linux; amd64

```console
$ docker pull haskell@sha256:060abd23f672a48371741fd92cf0733dd9cedcbfd320c091b6f7b742c8cecf06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **735.8 MB (735806219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642534eec3318ca53134b6f2f890c655dc0b679e6bb4ee2b4f2eccf8c64e0401`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:55:50 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:55:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:55:56 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba78c044035325832b13aaada4870fd8ff60e5dbf66e69cbfccbc6809a9c7cc`  
		Last Modified: Thu, 07 Sep 2023 04:07:23 GMT  
		Size: 400.2 MB (400231216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:51d604b8890a175bf4e838d83b609778483a57e138333555dc45335fdd4b7313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **798.0 MB (797974379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bc6a36fa738e8d8c7387b9727fefd41ffdc14f8f282c2d1a6a526a3097cbb7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC=9.2.8
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:17:31 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:17:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:17:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe7b5b4ef66f037e8f66916e5206891c9c35ba2a0e7b0b60e55493f7e14aa8`  
		Last Modified: Wed, 16 Aug 2023 03:26:09 GMT  
		Size: 465.4 MB (465430011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2-buster`

```console
$ docker pull haskell@sha256:21f26d54e749b7773c6a6df1ef27ec9a5310a22028c4e858f3a60251f4fac941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:060abd23f672a48371741fd92cf0733dd9cedcbfd320c091b6f7b742c8cecf06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **735.8 MB (735806219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642534eec3318ca53134b6f2f890c655dc0b679e6bb4ee2b4f2eccf8c64e0401`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:55:50 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:55:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:55:56 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba78c044035325832b13aaada4870fd8ff60e5dbf66e69cbfccbc6809a9c7cc`  
		Last Modified: Thu, 07 Sep 2023 04:07:23 GMT  
		Size: 400.2 MB (400231216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:51d604b8890a175bf4e838d83b609778483a57e138333555dc45335fdd4b7313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **798.0 MB (797974379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bc6a36fa738e8d8c7387b9727fefd41ffdc14f8f282c2d1a6a526a3097cbb7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC=9.2.8
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:17:31 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:17:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:17:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe7b5b4ef66f037e8f66916e5206891c9c35ba2a0e7b0b60e55493f7e14aa8`  
		Last Modified: Wed, 16 Aug 2023 03:26:09 GMT  
		Size: 465.4 MB (465430011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2-slim`

```console
$ docker pull haskell@sha256:d8e1938fcae839d3a9ffaf92e3e6402d053650d54d77c6e0156520a668966c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2-slim` - linux; amd64

```console
$ docker pull haskell@sha256:334562e75ed4d49b2cecd7e989d6df0f61c8e99271c89e4c506b6f3920e17fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422397431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39806a4b1c601793e38c86472e48285e465bdfd276da3fcc91ded05a037bf3f9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:56:12 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:56:13 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:57:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:57:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:57:30 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043aca5a9c2da0934b4c4eb7e979c1964f4689e80c63ab8a2a6e9d70e1c27965`  
		Last Modified: Thu, 07 Sep 2023 04:08:30 GMT  
		Size: 278.0 MB (277966812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:0e9c7ef7f250eec019b42060f47374c6f551082186df6ce8a9bfb1e5f2a75d69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.8 MB (463801503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c114839bca30febbecb80079a3fc968a7ac3e7916f5e8e9076e6f753042ad7`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:45:02 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:45:15 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:45:15 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec9b05ad6d6485bcf23d5ca4dbf9f477f23bc0a8e5a9c53a84ea1f31e3eb208`  
		Last Modified: Thu, 07 Sep 2023 01:49:48 GMT  
		Size: 320.2 MB (320176622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2-slim-buster`

```console
$ docker pull haskell@sha256:d8e1938fcae839d3a9ffaf92e3e6402d053650d54d77c6e0156520a668966c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:334562e75ed4d49b2cecd7e989d6df0f61c8e99271c89e4c506b6f3920e17fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422397431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39806a4b1c601793e38c86472e48285e465bdfd276da3fcc91ded05a037bf3f9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:56:12 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:56:13 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:57:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:57:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:57:30 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043aca5a9c2da0934b4c4eb7e979c1964f4689e80c63ab8a2a6e9d70e1c27965`  
		Last Modified: Thu, 07 Sep 2023 04:08:30 GMT  
		Size: 278.0 MB (277966812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:0e9c7ef7f250eec019b42060f47374c6f551082186df6ce8a9bfb1e5f2a75d69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.8 MB (463801503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c114839bca30febbecb80079a3fc968a7ac3e7916f5e8e9076e6f753042ad7`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:45:02 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:45:15 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:45:15 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec9b05ad6d6485bcf23d5ca4dbf9f477f23bc0a8e5a9c53a84ea1f31e3eb208`  
		Last Modified: Thu, 07 Sep 2023 01:49:48 GMT  
		Size: 320.2 MB (320176622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.8`

```console
$ docker pull haskell@sha256:21f26d54e749b7773c6a6df1ef27ec9a5310a22028c4e858f3a60251f4fac941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.8` - linux; amd64

```console
$ docker pull haskell@sha256:060abd23f672a48371741fd92cf0733dd9cedcbfd320c091b6f7b742c8cecf06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **735.8 MB (735806219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642534eec3318ca53134b6f2f890c655dc0b679e6bb4ee2b4f2eccf8c64e0401`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:55:50 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:55:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:55:56 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba78c044035325832b13aaada4870fd8ff60e5dbf66e69cbfccbc6809a9c7cc`  
		Last Modified: Thu, 07 Sep 2023 04:07:23 GMT  
		Size: 400.2 MB (400231216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.8` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:51d604b8890a175bf4e838d83b609778483a57e138333555dc45335fdd4b7313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **798.0 MB (797974379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bc6a36fa738e8d8c7387b9727fefd41ffdc14f8f282c2d1a6a526a3097cbb7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC=9.2.8
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:17:31 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:17:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:17:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe7b5b4ef66f037e8f66916e5206891c9c35ba2a0e7b0b60e55493f7e14aa8`  
		Last Modified: Wed, 16 Aug 2023 03:26:09 GMT  
		Size: 465.4 MB (465430011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.8-buster`

```console
$ docker pull haskell@sha256:21f26d54e749b7773c6a6df1ef27ec9a5310a22028c4e858f3a60251f4fac941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:060abd23f672a48371741fd92cf0733dd9cedcbfd320c091b6f7b742c8cecf06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **735.8 MB (735806219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642534eec3318ca53134b6f2f890c655dc0b679e6bb4ee2b4f2eccf8c64e0401`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:54:34 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:55:50 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:55:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:55:56 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba78c044035325832b13aaada4870fd8ff60e5dbf66e69cbfccbc6809a9c7cc`  
		Last Modified: Thu, 07 Sep 2023 04:07:23 GMT  
		Size: 400.2 MB (400231216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.8-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:51d604b8890a175bf4e838d83b609778483a57e138333555dc45335fdd4b7313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **798.0 MB (797974379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bc6a36fa738e8d8c7387b9727fefd41ffdc14f8f282c2d1a6a526a3097cbb7`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC=9.2.8
# Wed, 16 Aug 2023 03:16:08 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 16 Aug 2023 03:17:31 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 16 Aug 2023 03:17:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:17:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe7b5b4ef66f037e8f66916e5206891c9c35ba2a0e7b0b60e55493f7e14aa8`  
		Last Modified: Wed, 16 Aug 2023 03:26:09 GMT  
		Size: 465.4 MB (465430011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.8-slim`

```console
$ docker pull haskell@sha256:d8e1938fcae839d3a9ffaf92e3e6402d053650d54d77c6e0156520a668966c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.8-slim` - linux; amd64

```console
$ docker pull haskell@sha256:334562e75ed4d49b2cecd7e989d6df0f61c8e99271c89e4c506b6f3920e17fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422397431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39806a4b1c601793e38c86472e48285e465bdfd276da3fcc91ded05a037bf3f9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:56:12 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:56:13 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:57:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:57:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:57:30 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043aca5a9c2da0934b4c4eb7e979c1964f4689e80c63ab8a2a6e9d70e1c27965`  
		Last Modified: Thu, 07 Sep 2023 04:08:30 GMT  
		Size: 278.0 MB (277966812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.8-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:0e9c7ef7f250eec019b42060f47374c6f551082186df6ce8a9bfb1e5f2a75d69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.8 MB (463801503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c114839bca30febbecb80079a3fc968a7ac3e7916f5e8e9076e6f753042ad7`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:45:02 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:45:15 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:45:15 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec9b05ad6d6485bcf23d5ca4dbf9f477f23bc0a8e5a9c53a84ea1f31e3eb208`  
		Last Modified: Thu, 07 Sep 2023 01:49:48 GMT  
		Size: 320.2 MB (320176622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2.8-slim-buster`

```console
$ docker pull haskell@sha256:d8e1938fcae839d3a9ffaf92e3e6402d053650d54d77c6e0156520a668966c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.2.8-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:334562e75ed4d49b2cecd7e989d6df0f61c8e99271c89e4c506b6f3920e17fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422397431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39806a4b1c601793e38c86472e48285e465bdfd276da3fcc91ded05a037bf3f9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:56:12 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 03:56:13 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 03:57:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:57:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:57:30 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043aca5a9c2da0934b4c4eb7e979c1964f4689e80c63ab8a2a6e9d70e1c27965`  
		Last Modified: Thu, 07 Sep 2023 04:08:30 GMT  
		Size: 278.0 MB (277966812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.2.8-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:0e9c7ef7f250eec019b42060f47374c6f551082186df6ce8a9bfb1e5f2a75d69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.8 MB (463801503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c114839bca30febbecb80079a3fc968a7ac3e7916f5e8e9076e6f753042ad7`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC=9.2.8
# Thu, 07 Sep 2023 01:43:43 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Thu, 07 Sep 2023 01:45:02 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.2.8 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='645433359d8ad9e7b286f85ef5111db1b787ee3712c24c5dfde7c62769aa59a4';             ;;         'x86_64')             GHC_SHA256='10d1be25487bcf99ac8eb77beaa220c85e69f8c1106f4219ce019206ecc0ac51';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:45:15 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:45:15 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec9b05ad6d6485bcf23d5ca4dbf9f477f23bc0a8e5a9c53a84ea1f31e3eb208`  
		Last Modified: Thu, 07 Sep 2023 01:49:48 GMT  
		Size: 320.2 MB (320176622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4`

```console
$ docker pull haskell@sha256:a5eec7d86eb51b14b4d1c217dcc61abd1838faa71939a8bbbe3a1764f7e1c5c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4` - linux; amd64

```console
$ docker pull haskell@sha256:4265473a3abb399402810eb183e3697be455c424c3c13bfaa99667c771ed3a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **723.9 MB (723850372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0b345ed236886ce23fb5de5013f2b50cc801d69ba8955231f24f8531c8b58d`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:52:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:52:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:52:45 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79e556ae6d75f53855d43cd6cfcc34eb1c204f274f554269a273de80c0280b7`  
		Last Modified: Thu, 07 Sep 2023 04:04:51 GMT  
		Size: 388.3 MB (388275369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:987df9fb4d535a6bdb375117b30afffd517559d8fe3d33098f838c4b1e976e2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **768.9 MB (768944703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b980030937d64f7ce8693ceb6095cc1ac39eb6202c480cf48b68dc480ac7c400`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC=9.4.7
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Wed, 30 Aug 2023 23:40:55 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 30 Aug 2023 23:41:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Aug 2023 23:41:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8370c3cdd3ae9cf2c3aa2ebc7cc68f0489c6c114887d15f5fc04eb6fa421b`  
		Last Modified: Wed, 30 Aug 2023 23:44:21 GMT  
		Size: 436.4 MB (436400335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4-buster`

```console
$ docker pull haskell@sha256:a5eec7d86eb51b14b4d1c217dcc61abd1838faa71939a8bbbe3a1764f7e1c5c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:4265473a3abb399402810eb183e3697be455c424c3c13bfaa99667c771ed3a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **723.9 MB (723850372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0b345ed236886ce23fb5de5013f2b50cc801d69ba8955231f24f8531c8b58d`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:52:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:52:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:52:45 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79e556ae6d75f53855d43cd6cfcc34eb1c204f274f554269a273de80c0280b7`  
		Last Modified: Thu, 07 Sep 2023 04:04:51 GMT  
		Size: 388.3 MB (388275369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:987df9fb4d535a6bdb375117b30afffd517559d8fe3d33098f838c4b1e976e2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **768.9 MB (768944703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b980030937d64f7ce8693ceb6095cc1ac39eb6202c480cf48b68dc480ac7c400`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC=9.4.7
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Wed, 30 Aug 2023 23:40:55 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 30 Aug 2023 23:41:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Aug 2023 23:41:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8370c3cdd3ae9cf2c3aa2ebc7cc68f0489c6c114887d15f5fc04eb6fa421b`  
		Last Modified: Wed, 30 Aug 2023 23:44:21 GMT  
		Size: 436.4 MB (436400335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4-slim`

```console
$ docker pull haskell@sha256:d4c688b659493aa8e3351d46fd2136ab06cb4b544927774b260c8a3738fb82d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4-slim` - linux; amd64

```console
$ docker pull haskell@sha256:5eb890ba62d3678ce183e0438ea6e63f76c4115456faf9b89d0a04aa29a6703f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.4 MB (414371732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b2ad90c14a82e13f6ebe343217ee432675b82a0c4a6d1c0dd01b267872693f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:54:16 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:54:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:54:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7272189117f8e6290ce986316028c405bdedd2664322b56fc4076600bac7a4ba`  
		Last Modified: Thu, 07 Sep 2023 04:05:53 GMT  
		Size: 269.9 MB (269941113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:822ac75a6d69d12a64aedfc50226be9313cff0d08689064715a014f55b0857c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.9 MB (436914957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b64c11240bbf80351824eb1a2fcfbd6276bddd21280e867ada816357b8100f4`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 01:43:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:43:29 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:43:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c756f49e503bcceb8a845a434b9fa73afe8fc74a490d6faade4193d46aaf7e`  
		Last Modified: Thu, 07 Sep 2023 01:48:43 GMT  
		Size: 293.3 MB (293290076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4-slim-buster`

```console
$ docker pull haskell@sha256:d4c688b659493aa8e3351d46fd2136ab06cb4b544927774b260c8a3738fb82d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5eb890ba62d3678ce183e0438ea6e63f76c4115456faf9b89d0a04aa29a6703f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.4 MB (414371732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b2ad90c14a82e13f6ebe343217ee432675b82a0c4a6d1c0dd01b267872693f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:54:16 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:54:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:54:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7272189117f8e6290ce986316028c405bdedd2664322b56fc4076600bac7a4ba`  
		Last Modified: Thu, 07 Sep 2023 04:05:53 GMT  
		Size: 269.9 MB (269941113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:822ac75a6d69d12a64aedfc50226be9313cff0d08689064715a014f55b0857c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.9 MB (436914957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b64c11240bbf80351824eb1a2fcfbd6276bddd21280e867ada816357b8100f4`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 01:43:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:43:29 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:43:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c756f49e503bcceb8a845a434b9fa73afe8fc74a490d6faade4193d46aaf7e`  
		Last Modified: Thu, 07 Sep 2023 01:48:43 GMT  
		Size: 293.3 MB (293290076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.7`

```console
$ docker pull haskell@sha256:a5eec7d86eb51b14b4d1c217dcc61abd1838faa71939a8bbbe3a1764f7e1c5c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.7` - linux; amd64

```console
$ docker pull haskell@sha256:4265473a3abb399402810eb183e3697be455c424c3c13bfaa99667c771ed3a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **723.9 MB (723850372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0b345ed236886ce23fb5de5013f2b50cc801d69ba8955231f24f8531c8b58d`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:52:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:52:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:52:45 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79e556ae6d75f53855d43cd6cfcc34eb1c204f274f554269a273de80c0280b7`  
		Last Modified: Thu, 07 Sep 2023 04:04:51 GMT  
		Size: 388.3 MB (388275369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.7` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:987df9fb4d535a6bdb375117b30afffd517559d8fe3d33098f838c4b1e976e2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **768.9 MB (768944703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b980030937d64f7ce8693ceb6095cc1ac39eb6202c480cf48b68dc480ac7c400`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC=9.4.7
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Wed, 30 Aug 2023 23:40:55 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 30 Aug 2023 23:41:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Aug 2023 23:41:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8370c3cdd3ae9cf2c3aa2ebc7cc68f0489c6c114887d15f5fc04eb6fa421b`  
		Last Modified: Wed, 30 Aug 2023 23:44:21 GMT  
		Size: 436.4 MB (436400335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.7-buster`

```console
$ docker pull haskell@sha256:a5eec7d86eb51b14b4d1c217dcc61abd1838faa71939a8bbbe3a1764f7e1c5c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.7-buster` - linux; amd64

```console
$ docker pull haskell@sha256:4265473a3abb399402810eb183e3697be455c424c3c13bfaa99667c771ed3a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **723.9 MB (723850372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0b345ed236886ce23fb5de5013f2b50cc801d69ba8955231f24f8531c8b58d`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:51:16 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:52:40 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:52:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:52:45 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79e556ae6d75f53855d43cd6cfcc34eb1c204f274f554269a273de80c0280b7`  
		Last Modified: Thu, 07 Sep 2023 04:04:51 GMT  
		Size: 388.3 MB (388275369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.7-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:987df9fb4d535a6bdb375117b30afffd517559d8fe3d33098f838c4b1e976e2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **768.9 MB (768944703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b980030937d64f7ce8693ceb6095cc1ac39eb6202c480cf48b68dc480ac7c400`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC=9.4.7
# Wed, 30 Aug 2023 23:39:34 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Wed, 30 Aug 2023 23:40:55 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 30 Aug 2023 23:41:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Aug 2023 23:41:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8370c3cdd3ae9cf2c3aa2ebc7cc68f0489c6c114887d15f5fc04eb6fa421b`  
		Last Modified: Wed, 30 Aug 2023 23:44:21 GMT  
		Size: 436.4 MB (436400335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.7-slim`

```console
$ docker pull haskell@sha256:d4c688b659493aa8e3351d46fd2136ab06cb4b544927774b260c8a3738fb82d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.7-slim` - linux; amd64

```console
$ docker pull haskell@sha256:5eb890ba62d3678ce183e0438ea6e63f76c4115456faf9b89d0a04aa29a6703f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.4 MB (414371732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b2ad90c14a82e13f6ebe343217ee432675b82a0c4a6d1c0dd01b267872693f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:54:16 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:54:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:54:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7272189117f8e6290ce986316028c405bdedd2664322b56fc4076600bac7a4ba`  
		Last Modified: Thu, 07 Sep 2023 04:05:53 GMT  
		Size: 269.9 MB (269941113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.7-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:822ac75a6d69d12a64aedfc50226be9313cff0d08689064715a014f55b0857c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.9 MB (436914957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b64c11240bbf80351824eb1a2fcfbd6276bddd21280e867ada816357b8100f4`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 01:43:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:43:29 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:43:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c756f49e503bcceb8a845a434b9fa73afe8fc74a490d6faade4193d46aaf7e`  
		Last Modified: Thu, 07 Sep 2023 01:48:43 GMT  
		Size: 293.3 MB (293290076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.4.7-slim-buster`

```console
$ docker pull haskell@sha256:d4c688b659493aa8e3351d46fd2136ab06cb4b544927774b260c8a3738fb82d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.4.7-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5eb890ba62d3678ce183e0438ea6e63f76c4115456faf9b89d0a04aa29a6703f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.4 MB (414371732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b2ad90c14a82e13f6ebe343217ee432675b82a0c4a6d1c0dd01b267872693f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 03:52:55 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 03:54:16 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:54:21 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:54:21 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7272189117f8e6290ce986316028c405bdedd2664322b56fc4076600bac7a4ba`  
		Last Modified: Thu, 07 Sep 2023 04:05:53 GMT  
		Size: 269.9 MB (269941113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.4.7-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:822ac75a6d69d12a64aedfc50226be9313cff0d08689064715a014f55b0857c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.9 MB (436914957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b64c11240bbf80351824eb1a2fcfbd6276bddd21280e867ada816357b8100f4`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC=9.4.7
# Thu, 07 Sep 2023 01:42:04 GMT
ARG GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4
# Thu, 07 Sep 2023 01:43:19 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.4.7 GHC_RELEASE_KEY=88b57fcf7db53b4db3bfa4b1588764fbe22d19c4 STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='05896fc4bc52c117d281eac9c621c6c3a0b14f9f9eed5e42cce5e1c4485c7623';             ;;         'x86_64')             GHC_SHA256='6b5b939d20b47475358993210738578071005669500810f28746bbd856ed878b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:43:29 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.4.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:43:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c756f49e503bcceb8a845a434b9fa73afe8fc74a490d6faade4193d46aaf7e`  
		Last Modified: Thu, 07 Sep 2023 01:48:43 GMT  
		Size: 293.3 MB (293290076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6-buster`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6-slim`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6-slim` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6-slim-buster`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6.2`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6.2` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6.2` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6.2-buster`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6.2-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6.2-slim`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6.2-slim` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6.2-slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.6.2-slim-buster`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9.6.2-slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9.6.2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:b0d95f0a11196c78817cc044b6f6c1afe3cbcd3646f48f36167619787b70bcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:5e2bad693477a20f48010501f3c52e14be8d438d47836c4d54633a5d789c6921
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.7 MB (759693336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ae9af9eaf9fc97000e045c3d4149f38ba1929d17b9ad8c2c4cebd7dbc5ef9`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:23 GMT
ADD file:d9c3e291731c1f06d615709ebc665a41f6d6355607d87ae00768e3be4b330bed in / 
# Thu, 07 Sep 2023 00:21:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:59:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:59:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:46:58 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:47:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:47:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:47:06 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:47:06 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:47:08 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:47:09 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:48:48 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:48:54 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:48:54 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017`  
		Last Modified: Thu, 07 Sep 2023 00:26:22 GMT  
		Size: 50.5 MB (50497598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 17.6 MB (17579550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5`  
		Last Modified: Thu, 07 Sep 2023 03:07:09 GMT  
		Size: 51.9 MB (51887218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e`  
		Last Modified: Thu, 07 Sep 2023 03:07:41 GMT  
		Size: 191.9 MB (191897265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3189f7fc797b28dc3d35a0008cc669849713f954feedadc46a75c5af1b348`  
		Last Modified: Thu, 07 Sep 2023 04:00:47 GMT  
		Size: 515.0 KB (515035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010926ae7a71fecacb32008e9caac79fadb3b86cf7101cbc544707db7ecfabe`  
		Last Modified: Thu, 07 Sep 2023 04:00:50 GMT  
		Size: 15.4 MB (15359958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2822114cd34bb5007d04f71064cf8f54891e367b82304d3fa80c2031a444e5e`  
		Last Modified: Thu, 07 Sep 2023 04:00:49 GMT  
		Size: 7.8 MB (7838379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768527f573d9bba2bbdd93b2013e08b9890ee0dd92795d4958f7634e643ece25`  
		Last Modified: Thu, 07 Sep 2023 04:02:06 GMT  
		Size: 424.1 MB (424118333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:latest` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:f99170aff459255881896f5ae34de34697ea378a938ab6ca171bfae463136fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.2 MB (764195542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7da6fd5c8527be677cdcf765faa2da23b20424ccaf010ae017da68e38a3c074`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:07 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 03:12:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libnuma-dev         libtinfo-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK=2.11.1
# Wed, 16 Aug 2023 03:12:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 16 Aug 2023 03:12:19 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL=3.8.1.0
# Wed, 16 Aug 2023 03:12:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Wed, 16 Aug 2023 03:12:21 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC=9.6.2
# Thu, 17 Aug 2023 21:39:31 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 17 Aug 2023 21:41:03 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 17 Aug 2023 21:41:18 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 21:41:18 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407ce0ead9165147c42712d21eea5452801da640254e3b366151c677bbe67a63`  
		Last Modified: Wed, 16 Aug 2023 03:22:20 GMT  
		Size: 517.2 KB (517175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff83f56772c93cd19493c9ac13fb4d19043234b2ccd3085b89dbd92076a0f549`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 17.2 MB (17230030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b59e2d67f005996aa57c1d0c2940afa3eb58df22620a5de329e9babe01cd42`  
		Last Modified: Wed, 16 Aug 2023 03:22:22 GMT  
		Size: 12.4 MB (12373194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f45cbb3fe60a87ecb86f66a9d37c418b496fdcf31a3d10c049dc0c85015863`  
		Last Modified: Thu, 17 Aug 2023 21:44:49 GMT  
		Size: 431.7 MB (431651174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:slim`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:slim` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:slim` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:slim-buster`

```console
$ docker pull haskell@sha256:5c78bf0111454c21d55ef02c9c96c503de1ed9d9925f338b2d4878537a4112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:slim-buster` - linux; amd64

```console
$ docker pull haskell@sha256:592491a40e7512d2047c0f307966d2de1e18f522fd98929abea00a8760fbb073
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.2 MB (427216722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972f8c98ca228df601e89b6389beb4170ac1b3a13e367c296cf573a3edb66452`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:49:07 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 03:49:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 03:49:27 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 03:49:30 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 03:49:31 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 03:49:33 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 03:49:33 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 03:51:06 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 03:51:11 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:51:12 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bb617dd4aae8f28e1c4ce609aaae8b9784c07ede12d98bc73f24a1056eb10`  
		Last Modified: Thu, 07 Sep 2023 04:02:43 GMT  
		Size: 94.0 MB (94044918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8714307d10f302197b7d689304b8ba9c20b6cfaf589ad4227f827d9944f71aa4`  
		Last Modified: Thu, 07 Sep 2023 04:02:31 GMT  
		Size: 15.4 MB (15359954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb894b50d8472c8147f909e1cf4d1c13a3ca349cc0b11d4c905ab89712a394`  
		Last Modified: Thu, 07 Sep 2023 04:02:30 GMT  
		Size: 7.8 MB (7838362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e3b8ed42df935995a82666537c900915d28f944c160422711b6adee306c957`  
		Last Modified: Thu, 07 Sep 2023 04:03:20 GMT  
		Size: 282.8 MB (282786103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:slim-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:b5370bf4be0a6ae31167a3fabcf4f48558b453366e430afa9aff7d56f6ce39ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433544616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df07a46e840d53e4e7b910746e70ed8eb5ce08bdd861b72b36311a6de3c91da8`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:54 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 01:40:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libtinfo-dev         make         netbase         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK=2.11.1
# Thu, 07 Sep 2023 01:40:18 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 07 Sep 2023 01:40:22 GMT
# ARGS: STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             STACK_SHA256='c7733d07ed78d6f4d82e0ebf6d260eb693c6c9df2208003d60caba69766f9c15';             ;;         'x86_64')             STACK_SHA256='408a120e824ed6e6b24c548a2ff6f210fcb0eed246f204a280ed4c75af0517e7';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$STACK_URL" -o stack.tar.gz;     echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;         curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";     gpg --batch --verify stack.tar.gz.asc stack.tar.gz;     gpgconf --kill all;         tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";     stack config set system-ghc --global true;     stack config set install-ghc --global false;         rm -rf /tmp/*;         stack --version;
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL=3.8.1.0
# Thu, 07 Sep 2023 01:40:22 GMT
ARG CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C
# Thu, 07 Sep 2023 01:40:24 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='c7fa9029f2f829432dd9dcf764e58605fbb7431db79234feb3e46684a9b37214';             ;;         'x86_64')             CABAL_INSTALL_SHA256='c71a1a46fd42d235bb86be968660815c24950e5da2d1ff4640da025ab520424b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC=9.6.2
# Thu, 07 Sep 2023 01:40:25 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Thu, 07 Sep 2023 01:41:47 GMT
# ARGS: CABAL_INSTALL=3.8.1.0 CABAL_INSTALL_RELEASE_KEY=E9EC5616017C3EE26B33468CCE1ED8AE0B011D8C GHC=9.6.2 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.11.1 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='5ad6153718d23a025f0f547f099bcecdf325edb5f5e16a9ec8bdeb17bad3c128';             ;;         'x86_64')             GHC_SHA256='63d4bbcee19a343bcdb7bc7c6ca85b1f666a26c7a64fba9014d2160ec3d4ad20';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC-$ARCH-unknown-linux";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Thu, 07 Sep 2023 01:41:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.6.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:41:58 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ad0303ce58eddb47c58dcd0359386a120a72a7aa77689c36eb50b1274c878`  
		Last Modified: Thu, 07 Sep 2023 01:47:06 GMT  
		Size: 88.1 MB (88053900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3cef512deb5fc8f809414c4c358d633ea95af3184a5347b68e352f1985b8f`  
		Last Modified: Thu, 07 Sep 2023 01:47:03 GMT  
		Size: 17.2 MB (17230047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06a5826bd1c54c238339ff3dd9aacd185bbc174554cf2f29393ff7e70fc7652`  
		Last Modified: Thu, 07 Sep 2023 01:46:57 GMT  
		Size: 12.4 MB (12373186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0dc428fc126692e333c482967c42c43242e298251184d667228579b443990`  
		Last Modified: Thu, 07 Sep 2023 01:47:39 GMT  
		Size: 289.9 MB (289919735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
