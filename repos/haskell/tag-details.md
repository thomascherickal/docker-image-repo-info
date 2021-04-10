<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8-buster`](#haskell8-buster)
-	[`haskell:8-stretch`](#haskell8-stretch)
-	[`haskell:8.10`](#haskell810)
-	[`haskell:8.10-buster`](#haskell810-buster)
-	[`haskell:8.10-stretch`](#haskell810-stretch)
-	[`haskell:8.10.4`](#haskell8104)
-	[`haskell:8.10.4-buster`](#haskell8104-buster)
-	[`haskell:8.10.4-stretch`](#haskell8104-stretch)
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
$ docker pull haskell@sha256:457b1d4a3007017c32e0cff10e1debfaba1aadcb43f2a7976b5e1e9cbe313806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:5974cc970f3b7b1afdd09b67e7bdce1f1041d1696d53948cff6695844ea1a547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357612701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d650714e84566987efbeb802f672d373c4e0a613d5b1a945c2cb5ec592790d32`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:31 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:42:31 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:42:31 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:43:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:31 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:43:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:43:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1bbc6577af75cfdbf4cdf7d6c100d80752ebea928c8004b1f3fbb94fb1cd98`  
		Last Modified: Sat, 10 Apr 2021 06:49:43 GMT  
		Size: 278.8 MB (278763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f1456d3497c0c183127951385bf03301c2b80a6c3bb9cbc5405ad1bfc580d`  
		Last Modified: Sat, 10 Apr 2021 06:48:38 GMT  
		Size: 14.6 MB (14562640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:457b1d4a3007017c32e0cff10e1debfaba1aadcb43f2a7976b5e1e9cbe313806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5974cc970f3b7b1afdd09b67e7bdce1f1041d1696d53948cff6695844ea1a547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357612701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d650714e84566987efbeb802f672d373c4e0a613d5b1a945c2cb5ec592790d32`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:31 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:42:31 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:42:31 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:43:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:31 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:43:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:43:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1bbc6577af75cfdbf4cdf7d6c100d80752ebea928c8004b1f3fbb94fb1cd98`  
		Last Modified: Sat, 10 Apr 2021 06:49:43 GMT  
		Size: 278.8 MB (278763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f1456d3497c0c183127951385bf03301c2b80a6c3bb9cbc5405ad1bfc580d`  
		Last Modified: Sat, 10 Apr 2021 06:48:38 GMT  
		Size: 14.6 MB (14562640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-stretch`

```console
$ docker pull haskell@sha256:a48d7b408b6ede914a2faac237afc64ed2dd7592bcaf938b691df9189571b5d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:76bb20addb1ec763da124e9a9779a87ca2802008be292a12151d9087ec8bb216
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337072775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803114ea6d22e5c6ffc641c1afe74f0a4ad48e91084a0462e5b282998abc0e4b`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:42 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:43:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:43:43 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:44:36 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:44:46 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:44:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:44:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c7a420afde50bff6179243ddd6c6a7eeed0c62e0bcdb843daaa289f7dbae23`  
		Last Modified: Sat, 10 Apr 2021 06:51:13 GMT  
		Size: 267.5 MB (267543075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4975aee320ea3c20492ce663a070ecc130b9ed0c7ea6908f900218cc995ef999`  
		Last Modified: Sat, 10 Apr 2021 06:50:16 GMT  
		Size: 14.6 MB (14562707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:457b1d4a3007017c32e0cff10e1debfaba1aadcb43f2a7976b5e1e9cbe313806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:5974cc970f3b7b1afdd09b67e7bdce1f1041d1696d53948cff6695844ea1a547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357612701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d650714e84566987efbeb802f672d373c4e0a613d5b1a945c2cb5ec592790d32`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:31 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:42:31 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:42:31 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:43:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:31 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:43:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:43:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1bbc6577af75cfdbf4cdf7d6c100d80752ebea928c8004b1f3fbb94fb1cd98`  
		Last Modified: Sat, 10 Apr 2021 06:49:43 GMT  
		Size: 278.8 MB (278763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f1456d3497c0c183127951385bf03301c2b80a6c3bb9cbc5405ad1bfc580d`  
		Last Modified: Sat, 10 Apr 2021 06:48:38 GMT  
		Size: 14.6 MB (14562640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:457b1d4a3007017c32e0cff10e1debfaba1aadcb43f2a7976b5e1e9cbe313806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5974cc970f3b7b1afdd09b67e7bdce1f1041d1696d53948cff6695844ea1a547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357612701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d650714e84566987efbeb802f672d373c4e0a613d5b1a945c2cb5ec592790d32`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:31 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:42:31 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:42:31 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:43:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:31 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:43:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:43:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1bbc6577af75cfdbf4cdf7d6c100d80752ebea928c8004b1f3fbb94fb1cd98`  
		Last Modified: Sat, 10 Apr 2021 06:49:43 GMT  
		Size: 278.8 MB (278763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f1456d3497c0c183127951385bf03301c2b80a6c3bb9cbc5405ad1bfc580d`  
		Last Modified: Sat, 10 Apr 2021 06:48:38 GMT  
		Size: 14.6 MB (14562640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-stretch`

```console
$ docker pull haskell@sha256:a48d7b408b6ede914a2faac237afc64ed2dd7592bcaf938b691df9189571b5d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:76bb20addb1ec763da124e9a9779a87ca2802008be292a12151d9087ec8bb216
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337072775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803114ea6d22e5c6ffc641c1afe74f0a4ad48e91084a0462e5b282998abc0e4b`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:42 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:43:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:43:43 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:44:36 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:44:46 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:44:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:44:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c7a420afde50bff6179243ddd6c6a7eeed0c62e0bcdb843daaa289f7dbae23`  
		Last Modified: Sat, 10 Apr 2021 06:51:13 GMT  
		Size: 267.5 MB (267543075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4975aee320ea3c20492ce663a070ecc130b9ed0c7ea6908f900218cc995ef999`  
		Last Modified: Sat, 10 Apr 2021 06:50:16 GMT  
		Size: 14.6 MB (14562707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4`

```console
$ docker pull haskell@sha256:457b1d4a3007017c32e0cff10e1debfaba1aadcb43f2a7976b5e1e9cbe313806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.4` - linux; amd64

```console
$ docker pull haskell@sha256:5974cc970f3b7b1afdd09b67e7bdce1f1041d1696d53948cff6695844ea1a547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357612701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d650714e84566987efbeb802f672d373c4e0a613d5b1a945c2cb5ec592790d32`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:31 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:42:31 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:42:31 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:43:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:31 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:43:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:43:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1bbc6577af75cfdbf4cdf7d6c100d80752ebea928c8004b1f3fbb94fb1cd98`  
		Last Modified: Sat, 10 Apr 2021 06:49:43 GMT  
		Size: 278.8 MB (278763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f1456d3497c0c183127951385bf03301c2b80a6c3bb9cbc5405ad1bfc580d`  
		Last Modified: Sat, 10 Apr 2021 06:48:38 GMT  
		Size: 14.6 MB (14562640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4-buster`

```console
$ docker pull haskell@sha256:457b1d4a3007017c32e0cff10e1debfaba1aadcb43f2a7976b5e1e9cbe313806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:5974cc970f3b7b1afdd09b67e7bdce1f1041d1696d53948cff6695844ea1a547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357612701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d650714e84566987efbeb802f672d373c4e0a613d5b1a945c2cb5ec592790d32`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:31 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:42:31 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:42:31 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:42:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:43:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:31 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:43:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:43:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1bbc6577af75cfdbf4cdf7d6c100d80752ebea928c8004b1f3fbb94fb1cd98`  
		Last Modified: Sat, 10 Apr 2021 06:49:43 GMT  
		Size: 278.8 MB (278763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f1456d3497c0c183127951385bf03301c2b80a6c3bb9cbc5405ad1bfc580d`  
		Last Modified: Sat, 10 Apr 2021 06:48:38 GMT  
		Size: 14.6 MB (14562640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4-stretch`

```console
$ docker pull haskell@sha256:a48d7b408b6ede914a2faac237afc64ed2dd7592bcaf938b691df9189571b5d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.4-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:76bb20addb1ec763da124e9a9779a87ca2802008be292a12151d9087ec8bb216
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337072775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803114ea6d22e5c6ffc641c1afe74f0a4ad48e91084a0462e5b282998abc0e4b`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:43:42 GMT
ARG GHC=8.10.4
# Sat, 10 Apr 2021 06:43:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:43:43 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:43:43 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:44:36 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:44:46 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:44:46 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:44:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c7a420afde50bff6179243ddd6c6a7eeed0c62e0bcdb843daaa289f7dbae23`  
		Last Modified: Sat, 10 Apr 2021 06:51:13 GMT  
		Size: 267.5 MB (267543075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4975aee320ea3c20492ce663a070ecc130b9ed0c7ea6908f900218cc995ef999`  
		Last Modified: Sat, 10 Apr 2021 06:50:16 GMT  
		Size: 14.6 MB (14562707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-stretch`

```console
$ docker pull haskell@sha256:6bf4df08915e178dbc514032d331c4f715a0337bce30c1845458ae03862388f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:12edd4414e1ab29f28c4fdec6608323ac870c4a57042a27dc9ac37db6d822a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4f7c75c8cb2561327a394431bae4860c4a193232667443601272d93e901939`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:41:16 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:41:17 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:41:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:42:08 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:15 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:42:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:42:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb1230c1469292c284b197e9534fd3a886f4a2737e6c1e59e094c7e7f905e7`  
		Last Modified: Sat, 10 Apr 2021 06:48:17 GMT  
		Size: 265.5 MB (265515583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a5806c2c0e0a050544356c0ad0962507e7f90b6582cc7ff8451292d0ddc8e`  
		Last Modified: Sat, 10 Apr 2021 06:47:17 GMT  
		Size: 14.6 MB (14562673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-stretch`

```console
$ docker pull haskell@sha256:6bf4df08915e178dbc514032d331c4f715a0337bce30c1845458ae03862388f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:12edd4414e1ab29f28c4fdec6608323ac870c4a57042a27dc9ac37db6d822a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4f7c75c8cb2561327a394431bae4860c4a193232667443601272d93e901939`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:41:16 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:41:17 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:41:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:42:08 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:15 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:42:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:42:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb1230c1469292c284b197e9534fd3a886f4a2737e6c1e59e094c7e7f905e7`  
		Last Modified: Sat, 10 Apr 2021 06:48:17 GMT  
		Size: 265.5 MB (265515583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a5806c2c0e0a050544356c0ad0962507e7f90b6582cc7ff8451292d0ddc8e`  
		Last Modified: Sat, 10 Apr 2021 06:47:17 GMT  
		Size: 14.6 MB (14562673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0.1` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-buster`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0.1-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-stretch`

```console
$ docker pull haskell@sha256:6bf4df08915e178dbc514032d331c4f715a0337bce30c1845458ae03862388f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0.1-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:12edd4414e1ab29f28c4fdec6608323ac870c4a57042a27dc9ac37db6d822a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4f7c75c8cb2561327a394431bae4860c4a193232667443601272d93e901939`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:41:16 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:41:17 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:41:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:42:08 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:15 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:42:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:42:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb1230c1469292c284b197e9534fd3a886f4a2737e6c1e59e094c7e7f905e7`  
		Last Modified: Sat, 10 Apr 2021 06:48:17 GMT  
		Size: 265.5 MB (265515583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a5806c2c0e0a050544356c0ad0962507e7f90b6582cc7ff8451292d0ddc8e`  
		Last Modified: Sat, 10 Apr 2021 06:47:17 GMT  
		Size: 14.6 MB (14562673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:79328e2196dd6c7868f0927d2075f85170472ff36b4e0c3d8f35904c4eec072a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:f4aad54642ced76f9bf3e7219772fc799b7cc6e3202f55d71f91984c623ec5d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1acce9b930b45508d9e6ebe7da6e2a0a2d0e853bf38ca9ccef89824f2f0b5f9`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:39:38 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:39:51 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:39:52 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:39:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:39:52 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:39:52 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:39:53 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:40:51 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:40:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:40:56 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:40:57 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6313355ce5f82950a283ba45aac39e85e69ccf6c39ce3fe91b79e439c3acb7db`  
		Last Modified: Sat, 10 Apr 2021 06:45:31 GMT  
		Size: 13.9 MB (13853287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569b92c70f04fc4a657ca7bc9e87d2ad045f273cd4fba7309a8a65ae8c72016`  
		Last Modified: Sat, 10 Apr 2021 06:46:40 GMT  
		Size: 276.7 MB (276717394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a397c0b7ee5f513f98d4ad5ca2ae1f042243d83b9133bcfdbfe576982f099`  
		Last Modified: Sat, 10 Apr 2021 06:45:33 GMT  
		Size: 14.6 MB (14562643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

```console
$ docker pull haskell@sha256:6bf4df08915e178dbc514032d331c4f715a0337bce30c1845458ae03862388f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:12edd4414e1ab29f28c4fdec6608323ac870c4a57042a27dc9ac37db6d822a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4f7c75c8cb2561327a394431bae4860c4a193232667443601272d93e901939`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:41:16 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:41:17 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:41:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:42:08 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:15 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:42:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:42:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb1230c1469292c284b197e9534fd3a886f4a2737e6c1e59e094c7e7f905e7`  
		Last Modified: Sat, 10 Apr 2021 06:48:17 GMT  
		Size: 265.5 MB (265515583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a5806c2c0e0a050544356c0ad0962507e7f90b6582cc7ff8451292d0ddc8e`  
		Last Modified: Sat, 10 Apr 2021 06:47:17 GMT  
		Size: 14.6 MB (14562673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
