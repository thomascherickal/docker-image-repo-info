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
