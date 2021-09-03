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
$ docker pull haskell@sha256:d6962bc66ce366f39f1e444b28daf8a415dac429c07a71caf6e1791340c2281f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:e87031916b8a8c24c3f5f108a7e155d205970ebe64f1cc58c4a2932b7aa679e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361184741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2946588defb66f3d327f53a206a210f4237696d214e43e041d72100f28ffbb`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:04 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:04 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:04 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:47:32 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:47:36 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:47:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:47:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:47:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3422f85a89dff038c0c80ba8305d0831d8e2e60b7f577984251d28b135f8298e`  
		Last Modified: Fri, 03 Sep 2021 06:51:40 GMT  
		Size: 176.6 MB (176593179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f979350ff97263a77d5ac1f48366e98d9ab32934b81e9f7e67a3480f5164062`  
		Last Modified: Fri, 03 Sep 2021 06:51:05 GMT  
		Size: 18.1 MB (18103457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:d6962bc66ce366f39f1e444b28daf8a415dac429c07a71caf6e1791340c2281f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e87031916b8a8c24c3f5f108a7e155d205970ebe64f1cc58c4a2932b7aa679e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361184741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2946588defb66f3d327f53a206a210f4237696d214e43e041d72100f28ffbb`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:04 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:04 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:04 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:47:32 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:47:36 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:47:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:47:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:47:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3422f85a89dff038c0c80ba8305d0831d8e2e60b7f577984251d28b135f8298e`  
		Last Modified: Fri, 03 Sep 2021 06:51:40 GMT  
		Size: 176.6 MB (176593179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f979350ff97263a77d5ac1f48366e98d9ab32934b81e9f7e67a3480f5164062`  
		Last Modified: Fri, 03 Sep 2021 06:51:05 GMT  
		Size: 18.1 MB (18103457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-stretch`

```console
$ docker pull haskell@sha256:84d10594dd5fc6dc6c7eb2ba9e56134246c7243bcbeab0fdda0051cd50f68a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:61cb40082aebf38e55e1208bb7e1d6b36813c7f5fe65f5e2292a9a5afcc27e63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.5 MB (340524429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4693098b6e5b805ed0e654d38a796ca3e2f59cba6c4ee58e5160921ce9d3c6d`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:46 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:47 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:47 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:48:16 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:48:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:48:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c53bf9616b3753237cfbb29711c16afb0d26de07fc29b0372ec65c56e4830c`  
		Last Modified: Fri, 03 Sep 2021 06:52:39 GMT  
		Size: 180.5 MB (180538561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783bc1217008fe5bc6767b9216d77097e0ea30ca335914df10af76cdac66c0a`  
		Last Modified: Fri, 03 Sep 2021 06:52:04 GMT  
		Size: 18.1 MB (18103479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:d6962bc66ce366f39f1e444b28daf8a415dac429c07a71caf6e1791340c2281f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:e87031916b8a8c24c3f5f108a7e155d205970ebe64f1cc58c4a2932b7aa679e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361184741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2946588defb66f3d327f53a206a210f4237696d214e43e041d72100f28ffbb`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:04 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:04 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:04 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:47:32 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:47:36 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:47:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:47:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:47:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3422f85a89dff038c0c80ba8305d0831d8e2e60b7f577984251d28b135f8298e`  
		Last Modified: Fri, 03 Sep 2021 06:51:40 GMT  
		Size: 176.6 MB (176593179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f979350ff97263a77d5ac1f48366e98d9ab32934b81e9f7e67a3480f5164062`  
		Last Modified: Fri, 03 Sep 2021 06:51:05 GMT  
		Size: 18.1 MB (18103457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:d6962bc66ce366f39f1e444b28daf8a415dac429c07a71caf6e1791340c2281f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e87031916b8a8c24c3f5f108a7e155d205970ebe64f1cc58c4a2932b7aa679e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361184741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2946588defb66f3d327f53a206a210f4237696d214e43e041d72100f28ffbb`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:04 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:04 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:04 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:47:32 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:47:36 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:47:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:47:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:47:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3422f85a89dff038c0c80ba8305d0831d8e2e60b7f577984251d28b135f8298e`  
		Last Modified: Fri, 03 Sep 2021 06:51:40 GMT  
		Size: 176.6 MB (176593179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f979350ff97263a77d5ac1f48366e98d9ab32934b81e9f7e67a3480f5164062`  
		Last Modified: Fri, 03 Sep 2021 06:51:05 GMT  
		Size: 18.1 MB (18103457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-stretch`

```console
$ docker pull haskell@sha256:84d10594dd5fc6dc6c7eb2ba9e56134246c7243bcbeab0fdda0051cd50f68a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:61cb40082aebf38e55e1208bb7e1d6b36813c7f5fe65f5e2292a9a5afcc27e63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.5 MB (340524429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4693098b6e5b805ed0e654d38a796ca3e2f59cba6c4ee58e5160921ce9d3c6d`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:46 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:47 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:47 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:48:16 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:48:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:48:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c53bf9616b3753237cfbb29711c16afb0d26de07fc29b0372ec65c56e4830c`  
		Last Modified: Fri, 03 Sep 2021 06:52:39 GMT  
		Size: 180.5 MB (180538561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783bc1217008fe5bc6767b9216d77097e0ea30ca335914df10af76cdac66c0a`  
		Last Modified: Fri, 03 Sep 2021 06:52:04 GMT  
		Size: 18.1 MB (18103479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4`

```console
$ docker pull haskell@sha256:d6962bc66ce366f39f1e444b28daf8a415dac429c07a71caf6e1791340c2281f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.4` - linux; amd64

```console
$ docker pull haskell@sha256:e87031916b8a8c24c3f5f108a7e155d205970ebe64f1cc58c4a2932b7aa679e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361184741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2946588defb66f3d327f53a206a210f4237696d214e43e041d72100f28ffbb`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:04 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:04 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:04 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:47:32 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:47:36 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:47:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:47:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:47:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3422f85a89dff038c0c80ba8305d0831d8e2e60b7f577984251d28b135f8298e`  
		Last Modified: Fri, 03 Sep 2021 06:51:40 GMT  
		Size: 176.6 MB (176593179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f979350ff97263a77d5ac1f48366e98d9ab32934b81e9f7e67a3480f5164062`  
		Last Modified: Fri, 03 Sep 2021 06:51:05 GMT  
		Size: 18.1 MB (18103457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4-buster`

```console
$ docker pull haskell@sha256:d6962bc66ce366f39f1e444b28daf8a415dac429c07a71caf6e1791340c2281f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:e87031916b8a8c24c3f5f108a7e155d205970ebe64f1cc58c4a2932b7aa679e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361184741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2946588defb66f3d327f53a206a210f4237696d214e43e041d72100f28ffbb`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:04 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:04 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:04 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:47:32 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:47:35 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:47:36 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:47:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:47:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:47:40 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3422f85a89dff038c0c80ba8305d0831d8e2e60b7f577984251d28b135f8298e`  
		Last Modified: Fri, 03 Sep 2021 06:51:40 GMT  
		Size: 176.6 MB (176593179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f979350ff97263a77d5ac1f48366e98d9ab32934b81e9f7e67a3480f5164062`  
		Last Modified: Fri, 03 Sep 2021 06:51:05 GMT  
		Size: 18.1 MB (18103457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4-stretch`

```console
$ docker pull haskell@sha256:84d10594dd5fc6dc6c7eb2ba9e56134246c7243bcbeab0fdda0051cd50f68a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:8.10.4-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:61cb40082aebf38e55e1208bb7e1d6b36813c7f5fe65f5e2292a9a5afcc27e63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.5 MB (340524429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4693098b6e5b805ed0e654d38a796ca3e2f59cba6c4ee58e5160921ce9d3c6d`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:47:46 GMT
ARG GHC=8.10.4
# Fri, 03 Sep 2021 06:47:47 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:47:47 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:48:16 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:48:19 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:48:26 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:48:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c53bf9616b3753237cfbb29711c16afb0d26de07fc29b0372ec65c56e4830c`  
		Last Modified: Fri, 03 Sep 2021 06:52:39 GMT  
		Size: 180.5 MB (180538561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4783bc1217008fe5bc6767b9216d77097e0ea30ca335914df10af76cdac66c0a`  
		Last Modified: Fri, 03 Sep 2021 06:52:04 GMT  
		Size: 18.1 MB (18103479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-stretch`

```console
$ docker pull haskell@sha256:d1fb8ee87425461305466132c3320ea45255869423cb1576b0911516bf7d0fc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:1989dcb50fa8b584545e14803b5ed7deab21a1801a5b0bdb532de3f1037bbde1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338504607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bc94c515b54414614399be926d8045aa8c9de1a4e35eb55401b75aeb544f20`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:12 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:46:13 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:46:13 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:46:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:46:50 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:46:50 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:46:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22becd7f8704ca844b2110ee36ab2ea4b5cd174461d9fd7f033b4b5eea5eb21f`  
		Last Modified: Fri, 03 Sep 2021 06:50:46 GMT  
		Size: 178.5 MB (178518741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7113c55219fb5fa5abcc48c2fd408dc55ca7b211512a9688899a72edd730c04c`  
		Last Modified: Fri, 03 Sep 2021 06:50:10 GMT  
		Size: 18.1 MB (18103477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-stretch`

```console
$ docker pull haskell@sha256:d1fb8ee87425461305466132c3320ea45255869423cb1576b0911516bf7d0fc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:1989dcb50fa8b584545e14803b5ed7deab21a1801a5b0bdb532de3f1037bbde1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338504607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bc94c515b54414614399be926d8045aa8c9de1a4e35eb55401b75aeb544f20`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:12 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:46:13 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:46:13 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:46:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:46:50 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:46:50 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:46:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22becd7f8704ca844b2110ee36ab2ea4b5cd174461d9fd7f033b4b5eea5eb21f`  
		Last Modified: Fri, 03 Sep 2021 06:50:46 GMT  
		Size: 178.5 MB (178518741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7113c55219fb5fa5abcc48c2fd408dc55ca7b211512a9688899a72edd730c04c`  
		Last Modified: Fri, 03 Sep 2021 06:50:10 GMT  
		Size: 18.1 MB (18103477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-buster`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1-buster` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-stretch`

```console
$ docker pull haskell@sha256:d1fb8ee87425461305466132c3320ea45255869423cb1576b0911516bf7d0fc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:9.0.1-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:1989dcb50fa8b584545e14803b5ed7deab21a1801a5b0bdb532de3f1037bbde1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338504607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bc94c515b54414614399be926d8045aa8c9de1a4e35eb55401b75aeb544f20`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:12 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:46:13 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:46:13 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:46:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:46:50 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:46:50 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:46:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22becd7f8704ca844b2110ee36ab2ea4b5cd174461d9fd7f033b4b5eea5eb21f`  
		Last Modified: Fri, 03 Sep 2021 06:50:46 GMT  
		Size: 178.5 MB (178518741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7113c55219fb5fa5abcc48c2fd408dc55ca7b211512a9688899a72edd730c04c`  
		Last Modified: Fri, 03 Sep 2021 06:50:10 GMT  
		Size: 18.1 MB (18103477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:b6cb58755d4470ef2cd86e88d613eeb08ae8bdf5a763aebcd3b0f4e02fcf70a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:de9efe461b77413a3d11f6c7f9cdf922866af4205c2b7e140049239f194cbfb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359141359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd774daf2b4abf562efff76267e587521750eee61617c49c7d598c891d4a01`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:26 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:44:55 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:56 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:44:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:44:57 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:45:28 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:45:31 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:45:32 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:45:38 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:45:38 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:45:39 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b701565c4534c6c27174d36a5b59b9feb79d074d4b428c545a010f0a074b98f`  
		Last Modified: Fri, 03 Sep 2021 06:49:27 GMT  
		Size: 116.1 MB (116052212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c3a0c8b3fcd79a672841f90e84c4b3f615cb8f819a851b5f15e3bc7e6e37d`  
		Last Modified: Fri, 03 Sep 2021 06:49:41 GMT  
		Size: 174.5 MB (174549791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbca2ffb23af610b3ae83d18c0f30de00d7b69ebc8c43788284b28a8800e048`  
		Last Modified: Fri, 03 Sep 2021 06:49:05 GMT  
		Size: 18.1 MB (18103463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

```console
$ docker pull haskell@sha256:d1fb8ee87425461305466132c3320ea45255869423cb1576b0911516bf7d0fc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:1989dcb50fa8b584545e14803b5ed7deab21a1801a5b0bdb532de3f1037bbde1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338504607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bc94c515b54414614399be926d8045aa8c9de1a4e35eb55401b75aeb544f20`
-	Default Command: `["ghci"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:45:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 06:46:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         g++         git         gnupg         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:12 GMT
ARG GHC=9.0.1
# Fri, 03 Sep 2021 06:46:13 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Fri, 03 Sep 2021 06:46:13 GMT
ARG CABAL_INSTALL=3.4
# Fri, 03 Sep 2021 06:46:40 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         ghc-${GHC} &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK=2.7.3
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Fri, 03 Sep 2021 06:46:44 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Fri, 03 Sep 2021 06:46:50 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 03 Sep 2021 06:46:50 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 06:46:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241550cd638811093e1e5fe5eda0826906963c22646bddeea4c52a513ea6fb6`  
		Last Modified: Fri, 03 Sep 2021 06:50:22 GMT  
		Size: 96.5 MB (96502592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22becd7f8704ca844b2110ee36ab2ea4b5cd174461d9fd7f033b4b5eea5eb21f`  
		Last Modified: Fri, 03 Sep 2021 06:50:46 GMT  
		Size: 178.5 MB (178518741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7113c55219fb5fa5abcc48c2fd408dc55ca7b211512a9688899a72edd730c04c`  
		Last Modified: Fri, 03 Sep 2021 06:50:10 GMT  
		Size: 18.1 MB (18103477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
