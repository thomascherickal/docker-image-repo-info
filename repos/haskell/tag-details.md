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
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.2`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.2` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.2-buster`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.2-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.2-stretch`

```console
$ docker pull haskell@sha256:fe06bb4bd81c88f90db67abb39f93ca37572b817ffae4d5cf1492dd8fd4377f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.2-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:08aae990562f01a94af79a7f531d58da849a07e89866524094052d720825dfd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336490376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7689406580061fe29f4581618af66dfc6c4a394071e3b2af0cb9ce9696699918`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:01:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:45 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:01:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:01:46 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:02:30 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:37 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:02:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:02:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2e1304c7c8499be2551505c3667e4ef22d4b759bcc4d25e73a67114cdb2e9`  
		Last Modified: Thu, 10 Sep 2020 06:08:44 GMT  
		Size: 9.6 MB (9563228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3161c51660c6a70a96e5f1672abb9a830cb49b256a852a510a3cef56aefd6a`  
		Last Modified: Thu, 10 Sep 2020 06:10:17 GMT  
		Size: 267.0 MB (267018155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e205412fef3485dd39278e959d790af5e61071c781543cecfc97d8efc7c43304`  
		Last Modified: Thu, 10 Sep 2020 06:08:48 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-stretch`

```console
$ docker pull haskell@sha256:fe06bb4bd81c88f90db67abb39f93ca37572b817ffae4d5cf1492dd8fd4377f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:08aae990562f01a94af79a7f531d58da849a07e89866524094052d720825dfd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336490376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7689406580061fe29f4581618af66dfc6c4a394071e3b2af0cb9ce9696699918`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:01:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:45 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:01:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:01:46 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:02:30 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:37 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:02:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:02:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2e1304c7c8499be2551505c3667e4ef22d4b759bcc4d25e73a67114cdb2e9`  
		Last Modified: Thu, 10 Sep 2020 06:08:44 GMT  
		Size: 9.6 MB (9563228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3161c51660c6a70a96e5f1672abb9a830cb49b256a852a510a3cef56aefd6a`  
		Last Modified: Thu, 10 Sep 2020 06:10:17 GMT  
		Size: 267.0 MB (267018155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e205412fef3485dd39278e959d790af5e61071c781543cecfc97d8efc7c43304`  
		Last Modified: Thu, 10 Sep 2020 06:08:48 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8`

```console
$ docker pull haskell@sha256:325f165f9630866517fb1d8b02d22e348c26ee6c9ec8875d91961ca8b38a7f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8` - linux; amd64

```console
$ docker pull haskell@sha256:d9a84fb63424263de07825143201fa9ba5ad709142efb052de3b09d21a60468c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357532667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15fe3a662c05dee2b0115ac5c63394f0fdd43093d226585f40e302ececa76cd`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:51 GMT
ARG GHC=8.8.4
# Thu, 10 Sep 2020 06:02:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:02:52 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:03:38 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:03:45 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:03:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:03:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1631702f9f46ca708e04bdaac0a97c880ca668f988a0050e1a3611621d16f76e`  
		Last Modified: Thu, 10 Sep 2020 06:11:53 GMT  
		Size: 278.8 MB (278765201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c15acd62a0c79ddaa10f0d9cc1d6836ef874a92a08ba97a346de69fa4864752`  
		Last Modified: Thu, 10 Sep 2020 06:10:29 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.4`

```console
$ docker pull haskell@sha256:325f165f9630866517fb1d8b02d22e348c26ee6c9ec8875d91961ca8b38a7f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.4` - linux; amd64

```console
$ docker pull haskell@sha256:d9a84fb63424263de07825143201fa9ba5ad709142efb052de3b09d21a60468c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357532667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15fe3a662c05dee2b0115ac5c63394f0fdd43093d226585f40e302ececa76cd`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:51 GMT
ARG GHC=8.8.4
# Thu, 10 Sep 2020 06:02:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:02:52 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:03:38 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:03:45 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:03:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:03:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1631702f9f46ca708e04bdaac0a97c880ca668f988a0050e1a3611621d16f76e`  
		Last Modified: Thu, 10 Sep 2020 06:11:53 GMT  
		Size: 278.8 MB (278765201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c15acd62a0c79ddaa10f0d9cc1d6836ef874a92a08ba97a346de69fa4864752`  
		Last Modified: Thu, 10 Sep 2020 06:10:29 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.4-buster`

```console
$ docker pull haskell@sha256:325f165f9630866517fb1d8b02d22e348c26ee6c9ec8875d91961ca8b38a7f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:d9a84fb63424263de07825143201fa9ba5ad709142efb052de3b09d21a60468c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357532667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15fe3a662c05dee2b0115ac5c63394f0fdd43093d226585f40e302ececa76cd`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:51 GMT
ARG GHC=8.8.4
# Thu, 10 Sep 2020 06:02:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:02:52 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:03:38 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:03:45 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:03:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:03:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1631702f9f46ca708e04bdaac0a97c880ca668f988a0050e1a3611621d16f76e`  
		Last Modified: Thu, 10 Sep 2020 06:11:53 GMT  
		Size: 278.8 MB (278765201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c15acd62a0c79ddaa10f0d9cc1d6836ef874a92a08ba97a346de69fa4864752`  
		Last Modified: Thu, 10 Sep 2020 06:10:29 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.4-stretch`

```console
$ docker pull haskell@sha256:a9516bfe612058b74d8e738699432c5771feb32bff3ee8293f4290a49e37c598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.4-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:75aa861b658dca3acc324a56622f56ebc7b786afefefe3eb9a2192f7c467f66b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334362813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93115d099908a144bc3a20751162c52a978c29d9b6453d83aef05304e175bf80`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:01:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:03:58 GMT
ARG GHC=8.8.4
# Thu, 10 Sep 2020 06:03:58 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:03:59 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:03:59 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:03:59 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:04:00 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:05:11 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:05:21 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:05:24 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:05:24 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2e1304c7c8499be2551505c3667e4ef22d4b759bcc4d25e73a67114cdb2e9`  
		Last Modified: Thu, 10 Sep 2020 06:08:44 GMT  
		Size: 9.6 MB (9563228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eae2edc9a40b5a5d616a9bd93386a704c120fc687768e917efa634a03fe863`  
		Last Modified: Thu, 10 Sep 2020 06:13:38 GMT  
		Size: 264.9 MB (264890585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7c51a7571bdfe2ad31e509114e012a2cbc0cbe394733eb1189177633689a77`  
		Last Modified: Thu, 10 Sep 2020 06:12:18 GMT  
		Size: 14.5 MB (14542274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8-buster`

```console
$ docker pull haskell@sha256:325f165f9630866517fb1d8b02d22e348c26ee6c9ec8875d91961ca8b38a7f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:d9a84fb63424263de07825143201fa9ba5ad709142efb052de3b09d21a60468c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357532667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15fe3a662c05dee2b0115ac5c63394f0fdd43093d226585f40e302ececa76cd`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:51 GMT
ARG GHC=8.8.4
# Thu, 10 Sep 2020 06:02:52 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:02:52 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:02:52 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:03:38 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:03:45 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:03:47 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:03:51 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1631702f9f46ca708e04bdaac0a97c880ca668f988a0050e1a3611621d16f76e`  
		Last Modified: Thu, 10 Sep 2020 06:11:53 GMT  
		Size: 278.8 MB (278765201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c15acd62a0c79ddaa10f0d9cc1d6836ef874a92a08ba97a346de69fa4864752`  
		Last Modified: Thu, 10 Sep 2020 06:10:29 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8-stretch`

```console
$ docker pull haskell@sha256:a9516bfe612058b74d8e738699432c5771feb32bff3ee8293f4290a49e37c598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:75aa861b658dca3acc324a56622f56ebc7b786afefefe3eb9a2192f7c467f66b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334362813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93115d099908a144bc3a20751162c52a978c29d9b6453d83aef05304e175bf80`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:01:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:03:58 GMT
ARG GHC=8.8.4
# Thu, 10 Sep 2020 06:03:58 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:03:59 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:03:59 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:03:59 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:04:00 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:05:11 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:05:21 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.8.4 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:05:24 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.8.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:05:24 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2e1304c7c8499be2551505c3667e4ef22d4b759bcc4d25e73a67114cdb2e9`  
		Last Modified: Thu, 10 Sep 2020 06:08:44 GMT  
		Size: 9.6 MB (9563228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eae2edc9a40b5a5d616a9bd93386a704c120fc687768e917efa634a03fe863`  
		Last Modified: Thu, 10 Sep 2020 06:13:38 GMT  
		Size: 264.9 MB (264890585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7c51a7571bdfe2ad31e509114e012a2cbc0cbe394733eb1189177633689a77`  
		Last Modified: Thu, 10 Sep 2020 06:12:18 GMT  
		Size: 14.5 MB (14542274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-stretch`

```console
$ docker pull haskell@sha256:fe06bb4bd81c88f90db67abb39f93ca37572b817ffae4d5cf1492dd8fd4377f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:08aae990562f01a94af79a7f531d58da849a07e89866524094052d720825dfd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336490376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7689406580061fe29f4581618af66dfc6c4a394071e3b2af0cb9ce9696699918`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:01:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:45 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:01:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:01:46 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:02:30 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:37 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:02:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:02:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2e1304c7c8499be2551505c3667e4ef22d4b759bcc4d25e73a67114cdb2e9`  
		Last Modified: Thu, 10 Sep 2020 06:08:44 GMT  
		Size: 9.6 MB (9563228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3161c51660c6a70a96e5f1672abb9a830cb49b256a852a510a3cef56aefd6a`  
		Last Modified: Thu, 10 Sep 2020 06:10:17 GMT  
		Size: 267.0 MB (267018155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e205412fef3485dd39278e959d790af5e61071c781543cecfc97d8efc7c43304`  
		Last Modified: Thu, 10 Sep 2020 06:08:48 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:8c3dfe26416a849d03cb83101ff327793a0614e62c888de09153615dd20126e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:f883cd047fe7efaa39bf5f235c49ff8cac424fe8ceed3532c1d1293d376c792d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357090094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fd2cbd6f879d4db8817a332bd63af7e83a49084eabd009033f9b55668eb27c`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:00:01 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:00:02 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:00:02 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:00:03 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:00:03 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:00:04 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:01:14 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:23 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:01:26 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:01:29 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f237748fb6cd0e9deff8fd6ba12f4f6738d0d4288fd50fde716a83b458a00e`  
		Last Modified: Thu, 10 Sep 2020 06:06:01 GMT  
		Size: 13.8 MB (13829286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58d60e01448c6001b9a7cad8dc888b3470d81c5ba3d35c52f09a94ab887fecc`  
		Last Modified: Thu, 10 Sep 2020 06:08:31 GMT  
		Size: 278.3 MB (278322634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd3541d1d00b4644e9bc726517aed2dfcff8e060a0726e1d694c6e92516990`  
		Last Modified: Thu, 10 Sep 2020 06:06:02 GMT  
		Size: 14.5 MB (14542261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

```console
$ docker pull haskell@sha256:fe06bb4bd81c88f90db67abb39f93ca37572b817ffae4d5cf1492dd8fd4377f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:08aae990562f01a94af79a7f531d58da849a07e89866524094052d720825dfd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336490376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7689406580061fe29f4581618af66dfc6c4a394071e3b2af0cb9ce9696699918`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:01:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:01:45 GMT
ARG GHC=8.10.2
# Thu, 10 Sep 2020 06:01:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 10 Sep 2020 06:01:46 GMT
ARG CABAL_INSTALL=3.2
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK=2.3.3
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 10 Sep 2020 06:01:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 10 Sep 2020 06:02:30 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:02:37 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.3.3 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 10 Sep 2020 06:02:40 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 06:02:42 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2e1304c7c8499be2551505c3667e4ef22d4b759bcc4d25e73a67114cdb2e9`  
		Last Modified: Thu, 10 Sep 2020 06:08:44 GMT  
		Size: 9.6 MB (9563228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3161c51660c6a70a96e5f1672abb9a830cb49b256a852a510a3cef56aefd6a`  
		Last Modified: Thu, 10 Sep 2020 06:10:17 GMT  
		Size: 267.0 MB (267018155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e205412fef3485dd39278e959d790af5e61071c781543cecfc97d8efc7c43304`  
		Last Modified: Thu, 10 Sep 2020 06:08:48 GMT  
		Size: 14.5 MB (14542267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
