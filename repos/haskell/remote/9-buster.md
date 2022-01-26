## `haskell:9-buster`

```console
$ docker pull haskell@sha256:f6abc21e10ed267019340791f084119a79f6fd6b2a7ac9f7d44c273f09ccee45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:92c3aaf5a7cdbd4c5c79888d4fc56afb27a8cebca7a91b6e7ee974e8659dac47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.4 MB (416393068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adf4f9f4ead2bfbfc6f1299e0dd993bdc5ff1299d29cecc91d5083060b33d7f9`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:18:33 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 08:18:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:18:58 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 26 Jan 2022 08:18:59 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 26 Jan 2022 08:19:24 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='d9acee67d4308bc5c22d27bee034d388cc4192a25deff9e7e491e2396572b030';             ;;         'x86_64')             CABAL_INSTALL_SHA256='4759b56e9257e02f29fa374a6b25d6cb2f9d80c7e3a55d4f678a8e570925641c';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 26 Jan 2022 08:19:24 GMT
ARG GHC=9.2.1
# Wed, 26 Jan 2022 08:19:24 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 26 Jan 2022 08:21:12 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 GHC=9.2.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='717d4246a8b407a807048ce6eddb2785aca2e4c73b6b634c01e1726f42d539a1';             ;;         'x86_64')             GHC_SHA256='53f1650ed092230480ff5750b94f409e5dfe66bd07ced00bbbcdf5d6b180234c';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 26 Jan 2022 08:21:16 GMT
ARG STACK=2.7.3
# Wed, 26 Jan 2022 08:21:16 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 26 Jan 2022 08:21:36 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 GHC=9.2.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='a6c090555fa1c64aa61c29aa4449765a51d79e870cf759cde192937cd614e72b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 26 Jan 2022 08:21:36 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 08:21:36 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b11771dae63b6d88762b8585ff365dc3a6ef00c357e93d863e1b45491ba157`  
		Last Modified: Wed, 26 Jan 2022 08:26:53 GMT  
		Size: 120.6 MB (120593399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933603a127d7b5efc50aa19ce5db02caa54a79f4bfa7959f679c093c464edac4`  
		Last Modified: Wed, 26 Jan 2022 08:26:37 GMT  
		Size: 10.0 MB (10032282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c117408879d49089b6adac5f28c7ec5600c0077fd9cf174e57e874ee5e7fa`  
		Last Modified: Wed, 26 Jan 2022 08:27:20 GMT  
		Size: 217.4 MB (217429059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f67b40ebd6ec6f8f89fe866c5e8ca01a03dcd80ec4323e731f25d3925dd83d`  
		Last Modified: Wed, 26 Jan 2022 08:26:39 GMT  
		Size: 17.9 MB (17901271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haskell:9-buster` - linux; arm64 variant v8

```console
$ docker pull haskell@sha256:9689caebfaf4aea8adf9da83e401ee3d799ff8665b92ecdbdf1ed634601f0ec0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.4 MB (378388888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2f0a2a8c969b1d3ab27daafb9ab03b4f90114d5fe0a98df4742ea3cb3f26bb6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:15:35 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 04:15:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dpkg-dev         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libnuma-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:15:55 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 26 Jan 2022 04:15:56 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 26 Jan 2022 04:16:35 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     CABAL_INSTALL_TAR="cabal-install-$CABAL_INSTALL-$ARCH-linux-deb10.tar.xz";     CABAL_INSTALL_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/$CABAL_INSTALL_TAR";     CABAL_INSTALL_SHA256SUMS_URL="https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS";     case "$ARCH" in         'aarch64')             CABAL_INSTALL_SHA256='d9acee67d4308bc5c22d27bee034d388cc4192a25deff9e7e491e2396572b030';             ;;         'x86_64')             CABAL_INSTALL_SHA256='4759b56e9257e02f29fa374a6b25d6cb2f9d80c7e3a55d4f678a8e570925641c';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'"; exit 1 ;;     esac;     curl -fSL "$CABAL_INSTALL_URL" -o cabal-install.tar.gz;     echo "$CABAL_INSTALL_SHA256 cabal-install.tar.gz" | sha256sum --strict --check;         curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL";     curl -sSLO "$CABAL_INSTALL_SHA256SUMS_URL.sig";     GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$CABAL_INSTALL_RELEASE_KEY";     gpg --batch --verify SHA256SUMS.sig SHA256SUMS;     grep "$CABAL_INSTALL_SHA256  $CABAL_INSTALL_TAR" SHA256SUMS;     gpgconf --kill all;         tar -xf cabal-install.tar.gz -C /usr/local/bin;         rm -rf /tmp/*;         cabal --version
# Wed, 26 Jan 2022 04:16:36 GMT
ARG GHC=9.2.1
# Wed, 26 Jan 2022 04:16:37 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 26 Jan 2022 04:17:57 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 GHC=9.2.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     GHC_URL="https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-$ARCH-deb10-linux.tar.xz";     case "$ARCH" in         'aarch64')             GHC_SHA256='717d4246a8b407a807048ce6eddb2785aca2e4c73b6b634c01e1726f42d539a1';             ;;         'x86_64')             GHC_SHA256='53f1650ed092230480ff5750b94f409e5dfe66bd07ced00bbbcdf5d6b180234c';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     curl -sSL "$GHC_URL" -o ghc.tar.xz;     echo "$GHC_SHA256 ghc.tar.xz" | sha256sum --strict --check;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;     curl -sSL "$GHC_URL.sig" -o ghc.tar.xz.sig;     gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$GHC_RELEASE_KEY";     gpg --batch --verify ghc.tar.xz.sig ghc.tar.xz;     gpgconf --kill all;         tar xf ghc.tar.xz;     cd "ghc-$GHC";     ./configure --prefix "/opt/ghc/$GHC";     make install;     find "/opt/ghc/$GHC/" \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete;     rm -rf "/opt/ghc/$GHC/share/";         rm -rf /tmp/*;         "/opt/ghc/$GHC/bin/ghc" --version
# Wed, 26 Jan 2022 04:17:58 GMT
ARG STACK=2.7.3
# Wed, 26 Jan 2022 04:17:59 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 26 Jan 2022 04:18:01 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 GHC=9.2.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
RUN set -eux;     cd /tmp;     ARCH="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)";     INSTALL_STACK="true";     STACK_URL="https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-$ARCH.tar.gz";     case "$ARCH" in         'aarch64')             INSTALL_STACK="false";             ;;         'x86_64')             STACK_SHA256='a6c090555fa1c64aa61c29aa4449765a51d79e870cf759cde192937cd614e72b';             ;;         *) echo >&2 "error: unsupported architecture '$ARCH'" ; exit 1 ;;     esac;     if [ "$INSTALL_STACK" = "true" ]; then         curl -sSL "$STACK_URL" -o stack.tar.gz;         echo "$STACK_SHA256 stack.tar.gz" | sha256sum --strict --check;                 curl -sSL "$STACK_URL.asc" -o stack.tar.gz.asc;         GNUPGHOME="$(mktemp -d)"; export GNUPGHOME;         gpg --batch --keyserver keyserver.ubuntu.com --receive-keys "$STACK_RELEASE_KEY";         gpg --batch --verify stack.tar.gz.asc stack.tar.gz;         gpgconf --kill all;                 tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 "stack-$STACK-linux-$ARCH/stack";         stack config set system-ghc --global true;         stack config set install-ghc --global false;                 rm -rf /tmp/*;                 stack --version;     fi
# Wed, 26 Jan 2022 04:18:01 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.2.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 04:18:02 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6fe0fe558076976bed313221155852b8ccc1be208764c0212d7dc5d26407de`  
		Last Modified: Wed, 26 Jan 2022 04:23:46 GMT  
		Size: 114.6 MB (114626494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1cc8b642eb6d3ba7a015fcb255408719406d22a77ec8774819c6cabe81e79`  
		Last Modified: Wed, 26 Jan 2022 04:23:35 GMT  
		Size: 17.0 MB (16983883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce3d9dda1eb2971ae5049de272bfaaf5d7d597ce7be7c93fdaa110f3740ca66`  
		Last Modified: Wed, 26 Jan 2022 04:24:11 GMT  
		Size: 197.6 MB (197555470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
