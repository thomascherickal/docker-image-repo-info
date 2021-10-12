<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8-buster`](#haskell8-buster)
-	[`haskell:8-stretch`](#haskell8-stretch)
-	[`haskell:8.10`](#haskell810)
-	[`haskell:8.10-buster`](#haskell810-buster)
-	[`haskell:8.10-stretch`](#haskell810-stretch)
-	[`haskell:8.10.7`](#haskell8107)
-	[`haskell:8.10.7-buster`](#haskell8107-buster)
-	[`haskell:8.10.7-stretch`](#haskell8107-stretch)
-	[`haskell:9`](#haskell9)
-	[`haskell:9-buster`](#haskell9-buster)
-	[`haskell:9-stretch`](#haskell9-stretch)
-	[`haskell:9.0`](#haskell90)
-	[`haskell:9.0-buster`](#haskell90-buster)
-	[`haskell:9.0-stretch`](#haskell90-stretch)
-	[`haskell:9.0.1`](#haskell901)
-	[`haskell:9.0.1-buster`](#haskell901-buster)
-	[`haskell:9.0.1-stretch`](#haskell901-stretch)
-	[`haskell:buster`](#haskellbuster)
-	[`haskell:latest`](#haskelllatest)
-	[`haskell:stretch`](#haskellstretch)

## `haskell:8`

```console
$ docker pull haskell@sha256:1bfdf97ffd5f0d7ad6c47852b3ca238fc53cb415429478e07634d4c2bc977c6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:e34524213f2fe484680e8e050c98d486358dc6e184c4c798bdf1428ab76bbfce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409692114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386c3b8fc246b0a2a12d0bb4a7a24f2338178233ea31e1b1ca36068327bfff61`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:02:25 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Tue, 12 Oct 2021 17:03:40 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:03:45 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:03:57 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:03:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:03:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e74c0664e24fd06ccab51492df7040683aaedd86d7a14d79a0d927664cc1c`  
		Last Modified: Tue, 12 Oct 2021 17:08:58 GMT  
		Size: 214.5 MB (214524293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f71dffbe426c4735e5bca9dd76483d7ea3497f3925dfd508319acf97d60ac`  
		Last Modified: Tue, 12 Oct 2021 17:08:15 GMT  
		Size: 17.9 MB (17901262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:1bfdf97ffd5f0d7ad6c47852b3ca238fc53cb415429478e07634d4c2bc977c6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e34524213f2fe484680e8e050c98d486358dc6e184c4c798bdf1428ab76bbfce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409692114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386c3b8fc246b0a2a12d0bb4a7a24f2338178233ea31e1b1ca36068327bfff61`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:02:25 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Tue, 12 Oct 2021 17:03:40 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:03:45 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:03:57 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:03:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:03:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e74c0664e24fd06ccab51492df7040683aaedd86d7a14d79a0d927664cc1c`  
		Last Modified: Tue, 12 Oct 2021 17:08:58 GMT  
		Size: 214.5 MB (214524293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f71dffbe426c4735e5bca9dd76483d7ea3497f3925dfd508319acf97d60ac`  
		Last Modified: Tue, 12 Oct 2021 17:08:15 GMT  
		Size: 17.9 MB (17901262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-stretch`

```console
$ docker pull haskell@sha256:2b3593d090dc93cff86548838f5e24b927cb82e005f9ed53a8227599a6bb2980
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:100f8fb7d7d8d64adb5e106fe8136b8d4cbdc03aeb2cbd145a7597d74b69bafb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.7 MB (379725145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543656bbc1b7a8908703ba99e9741b34c74fa5e79d1a3488329cc69721a332ca`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23
# Tue, 12 Oct 2021 17:05:07 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:05:22 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:05:22 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:05:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4689ca6f7ae2dbdbdf811f402b81437cf78f735d4db3f1e58864dcf90e2337e`  
		Last Modified: Tue, 12 Oct 2021 17:10:03 GMT  
		Size: 209.2 MB (209183289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995638cabb78a0f0ad835f91f1ba5c6de0fcbbf554ffe855d4d33b7c43ab8281`  
		Last Modified: Tue, 12 Oct 2021 17:09:21 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:1bfdf97ffd5f0d7ad6c47852b3ca238fc53cb415429478e07634d4c2bc977c6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:e34524213f2fe484680e8e050c98d486358dc6e184c4c798bdf1428ab76bbfce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409692114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386c3b8fc246b0a2a12d0bb4a7a24f2338178233ea31e1b1ca36068327bfff61`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:02:25 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Tue, 12 Oct 2021 17:03:40 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:03:45 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:03:57 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:03:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:03:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e74c0664e24fd06ccab51492df7040683aaedd86d7a14d79a0d927664cc1c`  
		Last Modified: Tue, 12 Oct 2021 17:08:58 GMT  
		Size: 214.5 MB (214524293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f71dffbe426c4735e5bca9dd76483d7ea3497f3925dfd508319acf97d60ac`  
		Last Modified: Tue, 12 Oct 2021 17:08:15 GMT  
		Size: 17.9 MB (17901262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:1bfdf97ffd5f0d7ad6c47852b3ca238fc53cb415429478e07634d4c2bc977c6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e34524213f2fe484680e8e050c98d486358dc6e184c4c798bdf1428ab76bbfce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409692114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386c3b8fc246b0a2a12d0bb4a7a24f2338178233ea31e1b1ca36068327bfff61`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:02:25 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Tue, 12 Oct 2021 17:03:40 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:03:45 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:03:57 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:03:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:03:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e74c0664e24fd06ccab51492df7040683aaedd86d7a14d79a0d927664cc1c`  
		Last Modified: Tue, 12 Oct 2021 17:08:58 GMT  
		Size: 214.5 MB (214524293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f71dffbe426c4735e5bca9dd76483d7ea3497f3925dfd508319acf97d60ac`  
		Last Modified: Tue, 12 Oct 2021 17:08:15 GMT  
		Size: 17.9 MB (17901262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-stretch`

```console
$ docker pull haskell@sha256:2b3593d090dc93cff86548838f5e24b927cb82e005f9ed53a8227599a6bb2980
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:100f8fb7d7d8d64adb5e106fe8136b8d4cbdc03aeb2cbd145a7597d74b69bafb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.7 MB (379725145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543656bbc1b7a8908703ba99e9741b34c74fa5e79d1a3488329cc69721a332ca`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23
# Tue, 12 Oct 2021 17:05:07 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:05:22 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:05:22 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:05:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4689ca6f7ae2dbdbdf811f402b81437cf78f735d4db3f1e58864dcf90e2337e`  
		Last Modified: Tue, 12 Oct 2021 17:10:03 GMT  
		Size: 209.2 MB (209183289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995638cabb78a0f0ad835f91f1ba5c6de0fcbbf554ffe855d4d33b7c43ab8281`  
		Last Modified: Tue, 12 Oct 2021 17:09:21 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7`

```console
$ docker pull haskell@sha256:1bfdf97ffd5f0d7ad6c47852b3ca238fc53cb415429478e07634d4c2bc977c6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.7` - linux; amd64

```console
$ docker pull haskell@sha256:e34524213f2fe484680e8e050c98d486358dc6e184c4c798bdf1428ab76bbfce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409692114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386c3b8fc246b0a2a12d0bb4a7a24f2338178233ea31e1b1ca36068327bfff61`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:02:25 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Tue, 12 Oct 2021 17:03:40 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:03:45 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:03:57 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:03:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:03:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e74c0664e24fd06ccab51492df7040683aaedd86d7a14d79a0d927664cc1c`  
		Last Modified: Tue, 12 Oct 2021 17:08:58 GMT  
		Size: 214.5 MB (214524293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f71dffbe426c4735e5bca9dd76483d7ea3497f3925dfd508319acf97d60ac`  
		Last Modified: Tue, 12 Oct 2021 17:08:15 GMT  
		Size: 17.9 MB (17901262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7-buster`

```console
$ docker pull haskell@sha256:1bfdf97ffd5f0d7ad6c47852b3ca238fc53cb415429478e07634d4c2bc977c6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.7-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e34524213f2fe484680e8e050c98d486358dc6e184c4c798bdf1428ab76bbfce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409692114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386c3b8fc246b0a2a12d0bb4a7a24f2338178233ea31e1b1ca36068327bfff61`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:02:24 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:02:25 GMT
ARG GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
# Tue, 12 Oct 2021 17:03:40 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:03:44 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:03:45 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:03:57 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=A13719BCA87A0D3AC0C7D4157A4E60887009A7F1A8DBE95C4759EC413E086D30 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:03:57 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:03:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e74c0664e24fd06ccab51492df7040683aaedd86d7a14d79a0d927664cc1c`  
		Last Modified: Tue, 12 Oct 2021 17:08:58 GMT  
		Size: 214.5 MB (214524293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f71dffbe426c4735e5bca9dd76483d7ea3497f3925dfd508319acf97d60ac`  
		Last Modified: Tue, 12 Oct 2021 17:08:15 GMT  
		Size: 17.9 MB (17901262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.7-stretch`

```console
$ docker pull haskell@sha256:2b3593d090dc93cff86548838f5e24b927cb82e005f9ed53a8227599a6bb2980
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.7-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:100f8fb7d7d8d64adb5e106fe8136b8d4cbdc03aeb2cbd145a7597d74b69bafb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.7 MB (379725145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:543656bbc1b7a8908703ba99e9741b34c74fa5e79d1a3488329cc69721a332ca`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC=8.10.7
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4
# Tue, 12 Oct 2021 17:04:02 GMT
ARG GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23
# Tue, 12 Oct 2021 17:05:07 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 588764FBE22D19C4 --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:05:11 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:05:22 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=8.10.7 GHC_RELEASE_KEY=88B57FCF7DB53B4DB3BFA4B1588764FBE22D19C4 GHC_RELEASE_SHA256=CED9870EA351AF64FB48274B81A664CDB6A9266775F1598A79CBB6FDD5770A23 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:05:22 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/8.10.7/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:05:23 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4689ca6f7ae2dbdbdf811f402b81437cf78f735d4db3f1e58864dcf90e2337e`  
		Last Modified: Tue, 12 Oct 2021 17:10:03 GMT  
		Size: 209.2 MB (209183289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995638cabb78a0f0ad835f91f1ba5c6de0fcbbf554ffe855d4d33b7c43ab8281`  
		Last Modified: Tue, 12 Oct 2021 17:09:21 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-stretch`

```console
$ docker pull haskell@sha256:544ff4b67f165b4f76bffcee74c68700f996f11526658fd9b2bd22f7060a2d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:34c311ac7a66006825886b5bfcfb7b83302671ce6169c75949e2961a54461c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374101837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c00dbe8cea4a82a7f56b07977e0ab8f6a03d79d080751d9f67f94a20ae4045`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
# Tue, 12 Oct 2021 17:01:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:02:09 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:02:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a17d55ad3a8802e8274822ca8d340108f54183b01fcb122e6b439125fc80d`  
		Last Modified: Tue, 12 Oct 2021 17:07:55 GMT  
		Size: 203.6 MB (203559992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9302490dff99d31fe51a41f0057829934019416655bae3290a2555bfb133286`  
		Last Modified: Tue, 12 Oct 2021 17:07:13 GMT  
		Size: 17.9 MB (17901248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-stretch`

```console
$ docker pull haskell@sha256:544ff4b67f165b4f76bffcee74c68700f996f11526658fd9b2bd22f7060a2d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:34c311ac7a66006825886b5bfcfb7b83302671ce6169c75949e2961a54461c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374101837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c00dbe8cea4a82a7f56b07977e0ab8f6a03d79d080751d9f67f94a20ae4045`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
# Tue, 12 Oct 2021 17:01:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:02:09 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:02:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a17d55ad3a8802e8274822ca8d340108f54183b01fcb122e6b439125fc80d`  
		Last Modified: Tue, 12 Oct 2021 17:07:55 GMT  
		Size: 203.6 MB (203559992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9302490dff99d31fe51a41f0057829934019416655bae3290a2555bfb133286`  
		Last Modified: Tue, 12 Oct 2021 17:07:13 GMT  
		Size: 17.9 MB (17901248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-buster`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1-buster` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-stretch`

```console
$ docker pull haskell@sha256:544ff4b67f165b4f76bffcee74c68700f996f11526658fd9b2bd22f7060a2d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:34c311ac7a66006825886b5bfcfb7b83302671ce6169c75949e2961a54461c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374101837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c00dbe8cea4a82a7f56b07977e0ab8f6a03d79d080751d9f67f94a20ae4045`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
# Tue, 12 Oct 2021 17:01:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:02:09 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:02:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a17d55ad3a8802e8274822ca8d340108f54183b01fcb122e6b439125fc80d`  
		Last Modified: Tue, 12 Oct 2021 17:07:55 GMT  
		Size: 203.6 MB (203559992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9302490dff99d31fe51a41f0057829934019416655bae3290a2555bfb133286`  
		Last Modified: Tue, 12 Oct 2021 17:07:13 GMT  
		Size: 17.9 MB (17901248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:89f0d522c8fbb745c2e8486edcc905f332f9b4a39a5ab39ad76f2854dff6b639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:07125fef8d4d2018e02d163617fe9258fe87e2ed0299eec07574e26977f14c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403317456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a5e98aaa3e865b59805508edae14a06ff5e71254c8be0f8aea5c7c7564b98e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:57:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:58:18 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 16:58:19 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 16:58:32 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 16:58:32 GMT
ARG GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
# Tue, 12 Oct 2021 16:59:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb10-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:00:04 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:00:10 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=C253E7EB62CC9DA6524C491C85EC8D3727C2CA6035A8653388E636AAA30A2A0F STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:00:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306bdaad3742a2569f852c1c4661828f791cb93b514c9dfd0a397ad2a6e3299e`  
		Last Modified: Tue, 12 Oct 2021 17:06:13 GMT  
		Size: 117.0 MB (117013839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e5bb0457010cb9f852bdab79f7f03ec9520b46e8ef8e2af39caa2c0d347e66`  
		Last Modified: Tue, 12 Oct 2021 17:05:56 GMT  
		Size: 9.8 MB (9816028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665fad8184b2233809f900e770e2992d3f9e9d5e5dd25e0ab103e74ef354d39c`  
		Last Modified: Tue, 12 Oct 2021 17:06:42 GMT  
		Size: 208.1 MB (208149638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8169e061eb2faffec7113df5a612f099d364faeba94e5ebf1cbadb6cad08a6f4`  
		Last Modified: Tue, 12 Oct 2021 17:05:59 GMT  
		Size: 17.9 MB (17901259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

```console
$ docker pull haskell@sha256:544ff4b67f165b4f76bffcee74c68700f996f11526658fd9b2bd22f7060a2d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:34c311ac7a66006825886b5bfcfb7b83302671ce6169c75949e2961a54461c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374101837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c00dbe8cea4a82a7f56b07977e0ab8f6a03d79d080751d9f67f94a20ae4045`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:00:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 17:00:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         git         gcc         gnupg         g++         libc6-dev         libffi-dev         libgmp-dev         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL=3.6.0.0
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210
# Tue, 12 Oct 2021 17:00:41 GMT
ARG CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
# Tue, 12 Oct 2021 17:00:50 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${CABAL_INSTALL_RELEASE_KEY} &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS &&     curl -fSLO https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/SHA256SUMS.sig &&     gpg --batch --trusted-key B3D9F94B8DCAE210 --verify SHA256SUMS.sig SHA256SUMS &&     curl -fSL https://downloads.haskell.org/~cabal/cabal-install-$CABAL_INSTALL/cabal-install-$CABAL_INSTALL-x86_64-linux.tar.xz -o cabal-install.tar.gz &&     echo "$CABAL_INSTALL_RELEASE_SHA256 cabal-install.tar.gz" | sha256sum --strict --check &&     tar -xf cabal-install.tar.gz -C /usr/local/bin &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC=9.0.1
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD
# Tue, 12 Oct 2021 17:00:50 GMT
ARG GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
# Tue, 12 Oct 2021 17:01:59 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5
RUN cd /tmp &&   export GNUPGHOME="$(mktemp -d)" &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz -o ghc.tar.xz &&   curl -sSL https://downloads.haskell.org/~ghc/$GHC/ghc-$GHC-x86_64-deb9-linux.tar.xz.sig -o ghc.tar.xz.sig &&   gpg --batch --keyserver keyserver.ubuntu.com --receive-keys ${GHC_RELEASE_KEY} &&   gpg --batch --trusted-key 2DE04D4E97DB64AD --verify ghc.tar.xz.sig ghc.tar.xz &&   echo "$GHC_RELEASE_SHA256 ghc.tar.xz" | sha256sum --strict --check &&   tar xf ghc.tar.xz &&   cd ghc-$GHC &&   ./configure --prefix /opt/ghc/$GHC &&   make install &&   find /opt/ghc/$GHC/ \( -name "*_p.a" -o -name "*.p_hi" \) -type f -delete &&   rm -rf /opt/ghc/$GHC/share/ &&   rm -rf "$GNUPGHOME" /tmp/*
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK=2.7.3
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 12 Oct 2021 17:02:03 GMT
ARG STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
# Tue, 12 Oct 2021 17:02:09 GMT
# ARGS: CABAL_INSTALL=3.6.0.0 CABAL_INSTALL_RELEASE_KEY=A970DF3AC3B9709706D74544B3D9F94B8DCAE210 CABAL_INSTALL_RELEASE_SHA256=BFCB7350966DAFE95051B5FC9FCB989C5708AB9E78191E71FC04647061668A11 GHC=9.0.1 GHC_RELEASE_KEY=FFEB7CE81E16A36B3E2DED6F2DE04D4E97DB64AD GHC_RELEASE_SHA256=4CA6252492F59FE589029FADCA4B6F922D6A9F0FF39D19A2BD9886FDE4E183D5 STACK=2.7.3 STACK_RELEASE_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_SHA256=A6C090555FA1C64AA61C29AA4449765A51D79E870CF759CDE192937CD614E72B
RUN cd /tmp &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     echo "$STACK_RELEASE_SHA256 stack.tar.gz" | sha256sum --strict --check &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 stack-$STACK-linux-x86_64/stack &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /tmp/*
# Tue, 12 Oct 2021 17:02:10 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 17:02:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ecbb4abc0889c2c8472ea1668a846a9645c6aac79ae1b9cb8f3963de371c6`  
		Last Modified: Tue, 12 Oct 2021 17:07:26 GMT  
		Size: 97.4 MB (97444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f5908cc1a5a432c08d67d0a7e697395664ac9ede6e94ebb3e2fb8f04e5b36`  
		Last Modified: Tue, 12 Oct 2021 17:07:12 GMT  
		Size: 9.8 MB (9816054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a17d55ad3a8802e8274822ca8d340108f54183b01fcb122e6b439125fc80d`  
		Last Modified: Tue, 12 Oct 2021 17:07:55 GMT  
		Size: 203.6 MB (203559992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9302490dff99d31fe51a41f0057829934019416655bae3290a2555bfb133286`  
		Last Modified: Tue, 12 Oct 2021 17:07:13 GMT  
		Size: 17.9 MB (17901248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
