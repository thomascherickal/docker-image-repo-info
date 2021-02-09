<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8.10`](#haskell810)
-	[`haskell:8.10.2`](#haskell8102)
-	[`haskell:8.10.2-buster`](#haskell8102-buster)
-	[`haskell:8.10.2-stretch`](#haskell8102-stretch)
-	[`haskell:8.10-buster`](#haskell810-buster)
-	[`haskell:8.10-stretch`](#haskell810-stretch)
-	[`haskell:8.8`](#haskell88)
-	[`haskell:8.8.4`](#haskell884)
-	[`haskell:8.8.4-buster`](#haskell884-buster)
-	[`haskell:8.8.4-stretch`](#haskell884-stretch)
-	[`haskell:8.8-buster`](#haskell88-buster)
-	[`haskell:8.8-stretch`](#haskell88-stretch)
-	[`haskell:8-buster`](#haskell8-buster)
-	[`haskell:8-stretch`](#haskell8-stretch)
-	[`haskell:buster`](#haskellbuster)
-	[`haskell:latest`](#haskelllatest)
-	[`haskell:stretch`](#haskellstretch)

## `haskell:8`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.2`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.2` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.2-buster`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.2-stretch`

```console
$ docker pull haskell@sha256:23dbd044c25bc731a0bd1d8c09fdd9bd7bab4edb70eb88ff548fa6da8d5b0a87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.2-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:c02fc6c6b807e3a1e83d443cfa3c795f19f03d08bdf8c65280d1b255e35adee8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336601282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14756136c6cb38f748da2c9ef3282894e0ccb5516b07b8b5d9790cd54e7c87a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:17:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:18:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:18:09 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:18:09 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:18:09 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:19:17 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:28 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:19:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:19:33 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec5c8b5c70fd04e4069b7007d02cfe4024bdb584add2d7b69af66b8c0f5d64`  
		Last Modified: Tue, 09 Feb 2021 06:24:41 GMT  
		Size: 9.6 MB (9564711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c57e46fa4dd3601c31956ad867241dc32d2f9b1dbfbbab179f46e5d8a7b62`  
		Last Modified: Tue, 09 Feb 2021 06:26:03 GMT  
		Size: 267.1 MB (267094165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d9f8058b3406e904490b5987381d750516506b817f651f76ed3879d6d3d35`  
		Last Modified: Tue, 09 Feb 2021 06:24:45 GMT  
		Size: 14.6 MB (14562521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-stretch`

```console
$ docker pull haskell@sha256:23dbd044c25bc731a0bd1d8c09fdd9bd7bab4edb70eb88ff548fa6da8d5b0a87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:c02fc6c6b807e3a1e83d443cfa3c795f19f03d08bdf8c65280d1b255e35adee8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336601282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14756136c6cb38f748da2c9ef3282894e0ccb5516b07b8b5d9790cd54e7c87a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:17:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:18:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:18:09 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:18:09 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:18:09 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:19:17 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:28 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:19:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:19:33 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec5c8b5c70fd04e4069b7007d02cfe4024bdb584add2d7b69af66b8c0f5d64`  
		Last Modified: Tue, 09 Feb 2021 06:24:41 GMT  
		Size: 9.6 MB (9564711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c57e46fa4dd3601c31956ad867241dc32d2f9b1dbfbbab179f46e5d8a7b62`  
		Last Modified: Tue, 09 Feb 2021 06:26:03 GMT  
		Size: 267.1 MB (267094165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d9f8058b3406e904490b5987381d750516506b817f651f76ed3879d6d3d35`  
		Last Modified: Tue, 09 Feb 2021 06:24:45 GMT  
		Size: 14.6 MB (14562521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8`

```console
$ docker pull haskell@sha256:804181dc1c27e4618166156931ca80e45cadbb6d572bc5a15157c1fcbd7dfb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8` - linux; amd64

```console
$ docker pull haskell@sha256:0f62d7e62181a26235844f00c73a6afb76bee8f8b777883101e2070ec47454ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357628658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72422c2565eac7dc1443d34541e3d9fc4b35f5139c78ab98b375d614a6a87ebe`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:42 GMT
ARG GHC=8.8.4
# Tue, 09 Feb 2021 06:19:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:19:43 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:19:43 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:20:53 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:21:03 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:21:06 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:21:06 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b84a333fae5619ebcffbc6eafa75c38b7c84e7d570ec734ce3a104391f354b3`  
		Last Modified: Tue, 09 Feb 2021 06:27:41 GMT  
		Size: 278.8 MB (278814973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855fd15bbc4bbe7a432dbb71ef1503b26e1491fa6e3a78180ceb3f710030756`  
		Last Modified: Tue, 09 Feb 2021 06:26:17 GMT  
		Size: 14.6 MB (14562484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.4`

```console
$ docker pull haskell@sha256:804181dc1c27e4618166156931ca80e45cadbb6d572bc5a15157c1fcbd7dfb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.4` - linux; amd64

```console
$ docker pull haskell@sha256:0f62d7e62181a26235844f00c73a6afb76bee8f8b777883101e2070ec47454ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357628658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72422c2565eac7dc1443d34541e3d9fc4b35f5139c78ab98b375d614a6a87ebe`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:42 GMT
ARG GHC=8.8.4
# Tue, 09 Feb 2021 06:19:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:19:43 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:19:43 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:20:53 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:21:03 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:21:06 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:21:06 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b84a333fae5619ebcffbc6eafa75c38b7c84e7d570ec734ce3a104391f354b3`  
		Last Modified: Tue, 09 Feb 2021 06:27:41 GMT  
		Size: 278.8 MB (278814973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855fd15bbc4bbe7a432dbb71ef1503b26e1491fa6e3a78180ceb3f710030756`  
		Last Modified: Tue, 09 Feb 2021 06:26:17 GMT  
		Size: 14.6 MB (14562484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.4-buster`

```console
$ docker pull haskell@sha256:804181dc1c27e4618166156931ca80e45cadbb6d572bc5a15157c1fcbd7dfb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:0f62d7e62181a26235844f00c73a6afb76bee8f8b777883101e2070ec47454ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357628658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72422c2565eac7dc1443d34541e3d9fc4b35f5139c78ab98b375d614a6a87ebe`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:42 GMT
ARG GHC=8.8.4
# Tue, 09 Feb 2021 06:19:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:19:43 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:19:43 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:20:53 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:21:03 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:21:06 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:21:06 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b84a333fae5619ebcffbc6eafa75c38b7c84e7d570ec734ce3a104391f354b3`  
		Last Modified: Tue, 09 Feb 2021 06:27:41 GMT  
		Size: 278.8 MB (278814973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855fd15bbc4bbe7a432dbb71ef1503b26e1491fa6e3a78180ceb3f710030756`  
		Last Modified: Tue, 09 Feb 2021 06:26:17 GMT  
		Size: 14.6 MB (14562484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.4-stretch`

```console
$ docker pull haskell@sha256:df8d726327a60e8d7a007a0339190a90151fe9bce27431063c59d21731724b28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.4-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:de57c687f8e39c9f892907113a1bc58c35e24470b8f537c15a88d6c7ae96ea13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.5 MB (334455214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f5ed0923b2762f10ee342d7a53d4460d569779a3a151eb1aff2b0b49bc225a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:17:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:18:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:21:16 GMT
ARG GHC=8.8.4
# Tue, 09 Feb 2021 06:21:16 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:21:17 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:21:17 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:21:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:21:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:22:26 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:22:34 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:22:36 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:22:38 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec5c8b5c70fd04e4069b7007d02cfe4024bdb584add2d7b69af66b8c0f5d64`  
		Last Modified: Tue, 09 Feb 2021 06:24:41 GMT  
		Size: 9.6 MB (9564711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b916796929889b1a2593a0014abc75091a51389800e6f5a7371dde420ea2da08`  
		Last Modified: Tue, 09 Feb 2021 06:29:20 GMT  
		Size: 264.9 MB (264948098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb29718057475bc257609ddb7c3cf791c8a8bef70ced178a7e56f4783bee413`  
		Last Modified: Tue, 09 Feb 2021 06:27:56 GMT  
		Size: 14.6 MB (14562520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8-buster`

```console
$ docker pull haskell@sha256:804181dc1c27e4618166156931ca80e45cadbb6d572bc5a15157c1fcbd7dfb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:0f62d7e62181a26235844f00c73a6afb76bee8f8b777883101e2070ec47454ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357628658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72422c2565eac7dc1443d34541e3d9fc4b35f5139c78ab98b375d614a6a87ebe`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:42 GMT
ARG GHC=8.8.4
# Tue, 09 Feb 2021 06:19:43 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:19:43 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:19:43 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:19:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:20:53 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:21:03 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:21:06 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:21:06 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b84a333fae5619ebcffbc6eafa75c38b7c84e7d570ec734ce3a104391f354b3`  
		Last Modified: Tue, 09 Feb 2021 06:27:41 GMT  
		Size: 278.8 MB (278814973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855fd15bbc4bbe7a432dbb71ef1503b26e1491fa6e3a78180ceb3f710030756`  
		Last Modified: Tue, 09 Feb 2021 06:26:17 GMT  
		Size: 14.6 MB (14562484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8-stretch`

```console
$ docker pull haskell@sha256:df8d726327a60e8d7a007a0339190a90151fe9bce27431063c59d21731724b28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:de57c687f8e39c9f892907113a1bc58c35e24470b8f537c15a88d6c7ae96ea13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.5 MB (334455214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f5ed0923b2762f10ee342d7a53d4460d569779a3a151eb1aff2b0b49bc225a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:17:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:18:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:21:16 GMT
ARG GHC=8.8.4
# Tue, 09 Feb 2021 06:21:16 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:21:17 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:21:17 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:21:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:21:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:22:26 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:22:34 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:22:36 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:22:38 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec5c8b5c70fd04e4069b7007d02cfe4024bdb584add2d7b69af66b8c0f5d64`  
		Last Modified: Tue, 09 Feb 2021 06:24:41 GMT  
		Size: 9.6 MB (9564711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b916796929889b1a2593a0014abc75091a51389800e6f5a7371dde420ea2da08`  
		Last Modified: Tue, 09 Feb 2021 06:29:20 GMT  
		Size: 264.9 MB (264948098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb29718057475bc257609ddb7c3cf791c8a8bef70ced178a7e56f4783bee413`  
		Last Modified: Tue, 09 Feb 2021 06:27:56 GMT  
		Size: 14.6 MB (14562520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-stretch`

```console
$ docker pull haskell@sha256:23dbd044c25bc731a0bd1d8c09fdd9bd7bab4edb70eb88ff548fa6da8d5b0a87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:c02fc6c6b807e3a1e83d443cfa3c795f19f03d08bdf8c65280d1b255e35adee8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336601282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14756136c6cb38f748da2c9ef3282894e0ccb5516b07b8b5d9790cd54e7c87a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:17:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:18:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:18:09 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:18:09 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:18:09 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:19:17 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:28 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:19:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:19:33 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec5c8b5c70fd04e4069b7007d02cfe4024bdb584add2d7b69af66b8c0f5d64`  
		Last Modified: Tue, 09 Feb 2021 06:24:41 GMT  
		Size: 9.6 MB (9564711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c57e46fa4dd3601c31956ad867241dc32d2f9b1dbfbbab179f46e5d8a7b62`  
		Last Modified: Tue, 09 Feb 2021 06:26:03 GMT  
		Size: 267.1 MB (267094165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d9f8058b3406e904490b5987381d750516506b817f651f76ed3879d6d3d35`  
		Last Modified: Tue, 09 Feb 2021 06:24:45 GMT  
		Size: 14.6 MB (14562521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:402350476ec37ec98e3cfbfc2a4c909fe89440930c837c5b94c38defa8b72797
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:8247a287caa68bfad30c75eb965d442b6130e7c5535afa956544e24adc9e7434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357201415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b539f485b07c0ae5d5503c03de8145771207c74dd605d75ae0dfe2d054306e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:16:21 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:16:21 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:16:22 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:16:22 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:16:23 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:17:33 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:17:42 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:17:45 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:17:46 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbc36d177ff8feb884eb1725868cc8d30fe593b1ecb2d39d02d84552190f72c`  
		Last Modified: Tue, 09 Feb 2021 06:23:08 GMT  
		Size: 13.9 MB (13851003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b2b16a761038f2f6c89a600ad954e8b49d5fec359974667996ec1a68f8e3b`  
		Last Modified: Tue, 09 Feb 2021 06:24:24 GMT  
		Size: 278.4 MB (278387719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b9888b9e03d0d9503159f5615f86a6d2f7728f3727bb8f0f7319a952de3543`  
		Last Modified: Tue, 09 Feb 2021 06:23:10 GMT  
		Size: 14.6 MB (14562495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

```console
$ docker pull haskell@sha256:23dbd044c25bc731a0bd1d8c09fdd9bd7bab4edb70eb88ff548fa6da8d5b0a87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:c02fc6c6b807e3a1e83d443cfa3c795f19f03d08bdf8c65280d1b255e35adee8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336601282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14756136c6cb38f748da2c9ef3282894e0ccb5516b07b8b5d9790cd54e7c87a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:17:54 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 06:18:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:18:09 GMT
ARG GHC=8.10.2
# Tue, 09 Feb 2021 06:18:09 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Tue, 09 Feb 2021 06:18:09 GMT
ARG CABAL_INSTALL=3.2
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK=2.5.1
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Tue, 09 Feb 2021 06:18:10 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Tue, 09 Feb 2021 06:19:17 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:19:28 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Tue, 09 Feb 2021 06:19:30 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 06:19:33 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec5c8b5c70fd04e4069b7007d02cfe4024bdb584add2d7b69af66b8c0f5d64`  
		Last Modified: Tue, 09 Feb 2021 06:24:41 GMT  
		Size: 9.6 MB (9564711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c57e46fa4dd3601c31956ad867241dc32d2f9b1dbfbbab179f46e5d8a7b62`  
		Last Modified: Tue, 09 Feb 2021 06:26:03 GMT  
		Size: 267.1 MB (267094165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d9f8058b3406e904490b5987381d750516506b817f651f76ed3879d6d3d35`  
		Last Modified: Tue, 09 Feb 2021 06:24:45 GMT  
		Size: 14.6 MB (14562521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
