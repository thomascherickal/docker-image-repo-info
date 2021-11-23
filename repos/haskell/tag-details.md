<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8-buster`](#haskell8-buster)
-	[`haskell:8.10`](#haskell810)
-	[`haskell:8.10-buster`](#haskell810-buster)
-	[`haskell:8.10.7`](#haskell8107)
-	[`haskell:8.10.7-buster`](#haskell8107-buster)
-	[`haskell:9`](#haskell9)
-	[`haskell:9-buster`](#haskell9-buster)
-	[`haskell:9.0`](#haskell90)
-	[`haskell:9.0-buster`](#haskell90-buster)
-	[`haskell:9.0.1`](#haskell901)
-	[`haskell:9.0.1-buster`](#haskell901-buster)
-	[`haskell:9.2`](#haskell92)
-	[`haskell:9.2-buster`](#haskell92-buster)
-	[`haskell:9.2.1`](#haskell921)
-	[`haskell:9.2.1-buster`](#haskell921-buster)
-	[`haskell:buster`](#haskellbuster)
-	[`haskell:latest`](#haskelllatest)

## `haskell:8`

```console
$ docker pull haskell@sha256:82ac8f76e8608ac4f99adf3f9464b4a005469978c343141d74e6fb173879a8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:2318b7bcb2c57047fba8e12725a44c13f3441b2fbd9c55f926c2b904ed3b27f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.9 MB (409908564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b193d3444f43c3a68f577f39bd9d67a28771c92379fb80fb82960cdc4771e6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC=8.10.7
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Wed, 17 Nov 2021 08:56:43 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:56:49 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:56:49 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:56:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf296fc4b8f708f3f0f6cb9eb6b2a6f8f46bad7894a6a97917073832840f54f`  
		Last Modified: Wed, 17 Nov 2021 08:59:31 GMT  
		Size: 214.5 MB (214525316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893dd2c062c5968a215775931140899d6fc473eadd0bcdff99e8cf063a31390b`  
		Last Modified: Wed, 17 Nov 2021 08:58:39 GMT  
		Size: 17.9 MB (17901258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:82ac8f76e8608ac4f99adf3f9464b4a005469978c343141d74e6fb173879a8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:2318b7bcb2c57047fba8e12725a44c13f3441b2fbd9c55f926c2b904ed3b27f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.9 MB (409908564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b193d3444f43c3a68f577f39bd9d67a28771c92379fb80fb82960cdc4771e6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC=8.10.7
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Wed, 17 Nov 2021 08:56:43 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:56:49 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:56:49 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:56:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf296fc4b8f708f3f0f6cb9eb6b2a6f8f46bad7894a6a97917073832840f54f`  
		Last Modified: Wed, 17 Nov 2021 08:59:31 GMT  
		Size: 214.5 MB (214525316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893dd2c062c5968a215775931140899d6fc473eadd0bcdff99e8cf063a31390b`  
		Last Modified: Wed, 17 Nov 2021 08:58:39 GMT  
		Size: 17.9 MB (17901258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:82ac8f76e8608ac4f99adf3f9464b4a005469978c343141d74e6fb173879a8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:2318b7bcb2c57047fba8e12725a44c13f3441b2fbd9c55f926c2b904ed3b27f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.9 MB (409908564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b193d3444f43c3a68f577f39bd9d67a28771c92379fb80fb82960cdc4771e6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC=8.10.7
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Wed, 17 Nov 2021 08:56:43 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:56:49 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:56:49 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:56:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf296fc4b8f708f3f0f6cb9eb6b2a6f8f46bad7894a6a97917073832840f54f`  
		Last Modified: Wed, 17 Nov 2021 08:59:31 GMT  
		Size: 214.5 MB (214525316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893dd2c062c5968a215775931140899d6fc473eadd0bcdff99e8cf063a31390b`  
		Last Modified: Wed, 17 Nov 2021 08:58:39 GMT  
		Size: 17.9 MB (17901258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:82ac8f76e8608ac4f99adf3f9464b4a005469978c343141d74e6fb173879a8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:2318b7bcb2c57047fba8e12725a44c13f3441b2fbd9c55f926c2b904ed3b27f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.9 MB (409908564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b193d3444f43c3a68f577f39bd9d67a28771c92379fb80fb82960cdc4771e6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC=8.10.7
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Wed, 17 Nov 2021 08:56:43 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:56:49 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:56:49 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:56:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf296fc4b8f708f3f0f6cb9eb6b2a6f8f46bad7894a6a97917073832840f54f`  
		Last Modified: Wed, 17 Nov 2021 08:59:31 GMT  
		Size: 214.5 MB (214525316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893dd2c062c5968a215775931140899d6fc473eadd0bcdff99e8cf063a31390b`  
		Last Modified: Wed, 17 Nov 2021 08:58:39 GMT  
		Size: 17.9 MB (17901258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7`

```console
$ docker pull haskell@sha256:82ac8f76e8608ac4f99adf3f9464b4a005469978c343141d74e6fb173879a8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.7` - linux; amd64

```console
$ docker pull haskell@sha256:2318b7bcb2c57047fba8e12725a44c13f3441b2fbd9c55f926c2b904ed3b27f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.9 MB (409908564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b193d3444f43c3a68f577f39bd9d67a28771c92379fb80fb82960cdc4771e6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC=8.10.7
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Wed, 17 Nov 2021 08:56:43 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:56:49 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:56:49 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:56:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf296fc4b8f708f3f0f6cb9eb6b2a6f8f46bad7894a6a97917073832840f54f`  
		Last Modified: Wed, 17 Nov 2021 08:59:31 GMT  
		Size: 214.5 MB (214525316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893dd2c062c5968a215775931140899d6fc473eadd0bcdff99e8cf063a31390b`  
		Last Modified: Wed, 17 Nov 2021 08:58:39 GMT  
		Size: 17.9 MB (17901258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7-buster`

```console
$ docker pull haskell@sha256:82ac8f76e8608ac4f99adf3f9464b4a005469978c343141d74e6fb173879a8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.7-buster` - linux; amd64

```console
$ docker pull haskell@sha256:2318b7bcb2c57047fba8e12725a44c13f3441b2fbd9c55f926c2b904ed3b27f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.9 MB (409908564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b193d3444f43c3a68f577f39bd9d67a28771c92379fb80fb82960cdc4771e6`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC=8.10.7
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Wed, 17 Nov 2021 08:55:05 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Wed, 17 Nov 2021 08:56:43 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:56:44 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:56:49 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:56:49 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:56:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf296fc4b8f708f3f0f6cb9eb6b2a6f8f46bad7894a6a97917073832840f54f`  
		Last Modified: Wed, 17 Nov 2021 08:59:31 GMT  
		Size: 214.5 MB (214525316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893dd2c062c5968a215775931140899d6fc473eadd0bcdff99e8cf063a31390b`  
		Last Modified: Wed, 17 Nov 2021 08:58:39 GMT  
		Size: 17.9 MB (17901258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-buster`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1-buster` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.2`

```console
$ docker pull haskell@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `haskell:9.2-buster`

```console
$ docker pull haskell@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `haskell:9.2.1`

```console
$ docker pull haskell@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `haskell:9.2.1-buster`

```console
$ docker pull haskell@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `haskell:buster`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:ed0816a197d84d39514036ddcd6501223883d337417ae9965471895c6ca4da55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:d1bd86e8c29f6bcd1e752cbd3900e1c78b46a6ef444bc0905ceca93f98ece7e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403498117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e1bad3025b93d8d8fe9d73db14e8099a3152d97b98183ea923cbc34eb0a646`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:52:11 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 08:52:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL=3.6.2.0
# Wed, 17 Nov 2021 08:52:49 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Wed, 17 Nov 2021 08:52:50 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
# Wed, 17 Nov 2021 08:53:03 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux-deb10.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:53:03 GMT
ARG GHC=9.0.1
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Wed, 17 Nov 2021 08:53:04 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Wed, 17 Nov 2021 08:54:42 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK=2.7.3
# Wed, 17 Nov 2021 08:54:46 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 17 Nov 2021 08:54:47 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Wed, 17 Nov 2021 08:54:53 GMT
# ARGS: CABAL_INSTALL=3.6.2.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=4759B56E9257E02F29FA374A6B25D6CB2F9D80C7E3A55D4F678A8E570925641C GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Wed, 17 Nov 2021 08:54:53 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 08:54:53 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda5b98c17df639a97d00cfd1853fc356847c5fe4b03814fd495f977da07d1e4`  
		Last Modified: Wed, 17 Nov 2021 08:57:35 GMT  
		Size: 117.0 MB (117012616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee40dd36b63f610f7e6291d15e7ab8a2be8722e60f20c74bdd3638cbf74499ac`  
		Last Modified: Wed, 17 Nov 2021 08:57:19 GMT  
		Size: 10.0 MB (10032276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09bf38dc3acf361911e10b3ce2180c6c7137585a14b095e67c6562edbdd8e6`  
		Last Modified: Wed, 17 Nov 2021 08:58:06 GMT  
		Size: 208.1 MB (208114868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257fc0876db30e75f6f8ee63dd074f785d30de9f1039ebe9e8ca93c635df4`  
		Last Modified: Wed, 17 Nov 2021 08:57:20 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
