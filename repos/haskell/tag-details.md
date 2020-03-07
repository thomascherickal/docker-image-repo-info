<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8.6`](#haskell86)
-	[`haskell:8.6.5`](#haskell865)
-	[`haskell:8.8`](#haskell88)
-	[`haskell:8.8.2`](#haskell882)
-	[`haskell:8.8.3`](#haskell883)
-	[`haskell:latest`](#haskelllatest)

## `haskell:8`

```console
$ docker pull haskell@sha256:c717839f4e7d384b99759f257c852d13359b23b254de0d03bb4512d70f951b94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:85584329097cb288997e4fd84c600722172a8feffbda4130099a6437fe95ff76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334119906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597e930f7b603688d193fe9fc5998e49201b0ed6ebd1cd97fa35a601e149f92b`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:30:54 GMT
ARG GHC=8.8.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG STACK=2.1.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG CABAL_INSTALL=3.0
# Fri, 06 Mar 2020 23:31:36 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:31:45 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:31:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:31:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc266907aac934fe2e995bd7e2a8fc9ba4a2052d8c8a279ac220468f53f9c25`  
		Last Modified: Fri, 06 Mar 2020 23:34:55 GMT  
		Size: 264.6 MB (264563264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be966d1b10312144865340e35a672731696cc6bdaea0ef29ce254ec3062c03c8`  
		Last Modified: Fri, 06 Mar 2020 23:34:08 GMT  
		Size: 14.6 MB (14567385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.6`

```console
$ docker pull haskell@sha256:b021123545eddf48c6938d29cd9c17a68c8abc0007fade564a14237497734cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.6` - linux; amd64

```console
$ docker pull haskell@sha256:6cf5107b649834ff8c0a198b80e13d955088829dbe78ca465ccd0cbc55b12115
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:879921d872b6ccb75767d1549051656965b009cb0391879b3888e23427d67cbd`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:33:02 GMT
ARG GHC=8.6.5
# Fri, 06 Mar 2020 23:33:02 GMT
ARG STACK=1.9.3
# Fri, 06 Mar 2020 23:33:02 GMT
ARG CABAL_INSTALL=2.4
# Fri, 06 Mar 2020 23:33:38 GMT
# ARGS: CABAL_INSTALL=2.4 GHC=8.6.5 STACK=1.9.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:33:43 GMT
# ARGS: CABAL_INSTALL=2.4 GHC=8.6.5 STACK=1.9.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:33:43 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.4/bin:/opt/ghc/8.6.5/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:33:43 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9cdb655f293bb990294e88920757c328b22a123ec173a976d12df9a5478a12`  
		Last Modified: Fri, 06 Mar 2020 23:41:01 GMT  
		Size: 234.9 MB (234902570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df24066d3669806edb9903c8c51011276bd932c5ee1ed3494737262e8aeeb5bf`  
		Last Modified: Fri, 06 Mar 2020 23:40:11 GMT  
		Size: 14.2 MB (14236337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.6.5`

```console
$ docker pull haskell@sha256:b021123545eddf48c6938d29cd9c17a68c8abc0007fade564a14237497734cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.6.5` - linux; amd64

```console
$ docker pull haskell@sha256:6cf5107b649834ff8c0a198b80e13d955088829dbe78ca465ccd0cbc55b12115
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:879921d872b6ccb75767d1549051656965b009cb0391879b3888e23427d67cbd`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:33:02 GMT
ARG GHC=8.6.5
# Fri, 06 Mar 2020 23:33:02 GMT
ARG STACK=1.9.3
# Fri, 06 Mar 2020 23:33:02 GMT
ARG CABAL_INSTALL=2.4
# Fri, 06 Mar 2020 23:33:38 GMT
# ARGS: CABAL_INSTALL=2.4 GHC=8.6.5 STACK=1.9.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:33:43 GMT
# ARGS: CABAL_INSTALL=2.4 GHC=8.6.5 STACK=1.9.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:33:43 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/2.4/bin:/opt/ghc/8.6.5/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:33:43 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9cdb655f293bb990294e88920757c328b22a123ec173a976d12df9a5478a12`  
		Last Modified: Fri, 06 Mar 2020 23:41:01 GMT  
		Size: 234.9 MB (234902570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df24066d3669806edb9903c8c51011276bd932c5ee1ed3494737262e8aeeb5bf`  
		Last Modified: Fri, 06 Mar 2020 23:40:11 GMT  
		Size: 14.2 MB (14236337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8`

```console
$ docker pull haskell@sha256:c717839f4e7d384b99759f257c852d13359b23b254de0d03bb4512d70f951b94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8` - linux; amd64

```console
$ docker pull haskell@sha256:85584329097cb288997e4fd84c600722172a8feffbda4130099a6437fe95ff76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334119906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597e930f7b603688d193fe9fc5998e49201b0ed6ebd1cd97fa35a601e149f92b`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:30:54 GMT
ARG GHC=8.8.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG STACK=2.1.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG CABAL_INSTALL=3.0
# Fri, 06 Mar 2020 23:31:36 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:31:45 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:31:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:31:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc266907aac934fe2e995bd7e2a8fc9ba4a2052d8c8a279ac220468f53f9c25`  
		Last Modified: Fri, 06 Mar 2020 23:34:55 GMT  
		Size: 264.6 MB (264563264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be966d1b10312144865340e35a672731696cc6bdaea0ef29ce254ec3062c03c8`  
		Last Modified: Fri, 06 Mar 2020 23:34:08 GMT  
		Size: 14.6 MB (14567385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.2`

```console
$ docker pull haskell@sha256:0a9e244c753e5c0a14ac8891bcaa29a2c345f67bdeb47090b09d9953fa5ec305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.2` - linux; amd64

```console
$ docker pull haskell@sha256:cfc92ba4934d7b77d42ca3da97fec26b09fc8da212db8f9605d4f34d342d737d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334100516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262427cfe2dbf70fb7b2f3d7391030b35db664e6c5055588a40ee23215409a7b`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:31:58 GMT
ARG GHC=8.8.2
# Fri, 06 Mar 2020 23:31:58 GMT
ARG STACK=2.1.3
# Fri, 06 Mar 2020 23:31:59 GMT
ARG CABAL_INSTALL=3.0
# Fri, 06 Mar 2020 23:32:42 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.2 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:32:48 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.2 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:32:50 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:32:52 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dcaf8ecf96471e03caad567b9643a31422389c09bc6a592ff725ff4bbfbc69`  
		Last Modified: Fri, 06 Mar 2020 23:39:49 GMT  
		Size: 264.5 MB (264543856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb66b5fee3ac430076e2081258bec78fe0554cc411456637311f3ee916705b9e`  
		Last Modified: Fri, 06 Mar 2020 23:35:04 GMT  
		Size: 14.6 MB (14567403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.3`

```console
$ docker pull haskell@sha256:c717839f4e7d384b99759f257c852d13359b23b254de0d03bb4512d70f951b94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.3` - linux; amd64

```console
$ docker pull haskell@sha256:85584329097cb288997e4fd84c600722172a8feffbda4130099a6437fe95ff76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334119906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597e930f7b603688d193fe9fc5998e49201b0ed6ebd1cd97fa35a601e149f92b`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:30:54 GMT
ARG GHC=8.8.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG STACK=2.1.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG CABAL_INSTALL=3.0
# Fri, 06 Mar 2020 23:31:36 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:31:45 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:31:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:31:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc266907aac934fe2e995bd7e2a8fc9ba4a2052d8c8a279ac220468f53f9c25`  
		Last Modified: Fri, 06 Mar 2020 23:34:55 GMT  
		Size: 264.6 MB (264563264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be966d1b10312144865340e35a672731696cc6bdaea0ef29ce254ec3062c03c8`  
		Last Modified: Fri, 06 Mar 2020 23:34:08 GMT  
		Size: 14.6 MB (14567385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:c717839f4e7d384b99759f257c852d13359b23b254de0d03bb4512d70f951b94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:85584329097cb288997e4fd84c600722172a8feffbda4130099a6437fe95ff76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334119906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597e930f7b603688d193fe9fc5998e49201b0ed6ebd1cd97fa35a601e149f92b`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 23:30:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:30:54 GMT
ARG GHC=8.8.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG STACK=2.1.3
# Fri, 06 Mar 2020 23:30:54 GMT
ARG CABAL_INSTALL=3.0
# Fri, 06 Mar 2020 23:31:36 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Fri, 06 Mar 2020 23:31:45 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Fri, 06 Mar 2020 23:31:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Mar 2020 23:31:49 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede929110a7b3758d4b51b350a9fcc5dcc8643cfb5494c7d55a9ea43e35ea082`  
		Last Modified: Fri, 06 Mar 2020 23:34:04 GMT  
		Size: 9.6 MB (9613325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc266907aac934fe2e995bd7e2a8fc9ba4a2052d8c8a279ac220468f53f9c25`  
		Last Modified: Fri, 06 Mar 2020 23:34:55 GMT  
		Size: 264.6 MB (264563264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be966d1b10312144865340e35a672731696cc6bdaea0ef29ce254ec3062c03c8`  
		Last Modified: Fri, 06 Mar 2020 23:34:08 GMT  
		Size: 14.6 MB (14567385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
