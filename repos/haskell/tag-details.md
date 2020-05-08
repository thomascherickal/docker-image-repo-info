<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haskell`

-	[`haskell:8`](#haskell8)
-	[`haskell:8.10`](#haskell810)
-	[`haskell:8.10.1`](#haskell8101)
-	[`haskell:8.10.1-buster`](#haskell8101-buster)
-	[`haskell:8.10.1-stretch`](#haskell8101-stretch)
-	[`haskell:8.10-buster`](#haskell810-buster)
-	[`haskell:8.10-stretch`](#haskell810-stretch)
-	[`haskell:8.8`](#haskell88)
-	[`haskell:8.8.3`](#haskell883)
-	[`haskell:8.8.3-buster`](#haskell883-buster)
-	[`haskell:8.8.3-stretch`](#haskell883-stretch)
-	[`haskell:8.8-buster`](#haskell88-buster)
-	[`haskell:8.8-stretch`](#haskell88-stretch)
-	[`haskell:8-buster`](#haskell8-buster)
-	[`haskell:8-stretch`](#haskell8-stretch)
-	[`haskell:buster`](#haskellbuster)
-	[`haskell:latest`](#haskelllatest)
-	[`haskell:stretch`](#haskellstretch)

## `haskell:8`

```console
$ docker pull haskell@sha256:7c8ff5c85fb0ad9ab1c63f578c31a52e5b9ce01d62e669702fba8dee2fa5cd30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:de98637baf65b997e63386f580e3bc7436b666385d6e28abc5d03746da995ff1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334111938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b595e371319cf0954a527ab340abe162aa577ed0a1a14f951b2b46ea0046f06f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:36:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:36:57 GMT
ARG GHC=8.8.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG STACK=2.1.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG CABAL_INSTALL=3.0
# Thu, 23 Apr 2020 01:37:57 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:38:06 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 23 Apr 2020 01:38:08 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 01:38:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d8700a62fa028e779c34a2981a9301bd2856a8383d8d2295586a2dc51e44bc`  
		Last Modified: Thu, 23 Apr 2020 01:39:19 GMT  
		Size: 9.6 MB (9613310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adbe3ddd630aa5727b4d0afc72c65882be19ca211d9f9cdd0404c9d4428c568`  
		Last Modified: Thu, 23 Apr 2020 01:40:23 GMT  
		Size: 264.6 MB (264555287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9cc3e6c95b5baabaa0992459a8c906c9690ac798578f3dc8df3036593ea`  
		Last Modified: Thu, 23 Apr 2020 01:39:22 GMT  
		Size: 14.6 MB (14567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

**does not exist** (yet?)

## `haskell:8.10.1`

**does not exist** (yet?)

## `haskell:8.10.1-buster`

**does not exist** (yet?)

## `haskell:8.10.1-stretch`

**does not exist** (yet?)

## `haskell:8.10-buster`

**does not exist** (yet?)

## `haskell:8.10-stretch`

**does not exist** (yet?)

## `haskell:8.8`

```console
$ docker pull haskell@sha256:7c8ff5c85fb0ad9ab1c63f578c31a52e5b9ce01d62e669702fba8dee2fa5cd30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8` - linux; amd64

```console
$ docker pull haskell@sha256:de98637baf65b997e63386f580e3bc7436b666385d6e28abc5d03746da995ff1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334111938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b595e371319cf0954a527ab340abe162aa577ed0a1a14f951b2b46ea0046f06f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:36:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:36:57 GMT
ARG GHC=8.8.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG STACK=2.1.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG CABAL_INSTALL=3.0
# Thu, 23 Apr 2020 01:37:57 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:38:06 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 23 Apr 2020 01:38:08 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 01:38:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d8700a62fa028e779c34a2981a9301bd2856a8383d8d2295586a2dc51e44bc`  
		Last Modified: Thu, 23 Apr 2020 01:39:19 GMT  
		Size: 9.6 MB (9613310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adbe3ddd630aa5727b4d0afc72c65882be19ca211d9f9cdd0404c9d4428c568`  
		Last Modified: Thu, 23 Apr 2020 01:40:23 GMT  
		Size: 264.6 MB (264555287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9cc3e6c95b5baabaa0992459a8c906c9690ac798578f3dc8df3036593ea`  
		Last Modified: Thu, 23 Apr 2020 01:39:22 GMT  
		Size: 14.6 MB (14567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.3`

```console
$ docker pull haskell@sha256:7c8ff5c85fb0ad9ab1c63f578c31a52e5b9ce01d62e669702fba8dee2fa5cd30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.8.3` - linux; amd64

```console
$ docker pull haskell@sha256:de98637baf65b997e63386f580e3bc7436b666385d6e28abc5d03746da995ff1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334111938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b595e371319cf0954a527ab340abe162aa577ed0a1a14f951b2b46ea0046f06f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:36:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:36:57 GMT
ARG GHC=8.8.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG STACK=2.1.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG CABAL_INSTALL=3.0
# Thu, 23 Apr 2020 01:37:57 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:38:06 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 23 Apr 2020 01:38:08 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 01:38:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d8700a62fa028e779c34a2981a9301bd2856a8383d8d2295586a2dc51e44bc`  
		Last Modified: Thu, 23 Apr 2020 01:39:19 GMT  
		Size: 9.6 MB (9613310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adbe3ddd630aa5727b4d0afc72c65882be19ca211d9f9cdd0404c9d4428c568`  
		Last Modified: Thu, 23 Apr 2020 01:40:23 GMT  
		Size: 264.6 MB (264555287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9cc3e6c95b5baabaa0992459a8c906c9690ac798578f3dc8df3036593ea`  
		Last Modified: Thu, 23 Apr 2020 01:39:22 GMT  
		Size: 14.6 MB (14567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.8.3-buster`

**does not exist** (yet?)

## `haskell:8.8.3-stretch`

**does not exist** (yet?)

## `haskell:8.8-buster`

**does not exist** (yet?)

## `haskell:8.8-stretch`

**does not exist** (yet?)

## `haskell:8-buster`

**does not exist** (yet?)

## `haskell:8-stretch`

**does not exist** (yet?)

## `haskell:buster`

**does not exist** (yet?)

## `haskell:latest`

```console
$ docker pull haskell@sha256:7c8ff5c85fb0ad9ab1c63f578c31a52e5b9ce01d62e669702fba8dee2fa5cd30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:de98637baf65b997e63386f580e3bc7436b666385d6e28abc5d03746da995ff1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334111938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b595e371319cf0954a527ab340abe162aa577ed0a1a14f951b2b46ea0046f06f`
-	Default Command: `["ghci"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:36:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:36:57 GMT
ARG GHC=8.8.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG STACK=2.1.3
# Thu, 23 Apr 2020 01:36:58 GMT
ARG CABAL_INSTALL=3.0
# Thu, 23 Apr 2020 01:37:57 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:38:06 GMT
# ARGS: CABAL_INSTALL=3.0 GHC=8.8.3 STACK=2.1.3
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys C5705533DA4F78D8664B5DC0575159689BEFB442 &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 2C6A674E85EE3FB896AFC9B965101FF31C5C154D &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 23 Apr 2020 01:38:08 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.0/bin:/opt/ghc/8.8.3/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 01:38:10 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d8700a62fa028e779c34a2981a9301bd2856a8383d8d2295586a2dc51e44bc`  
		Last Modified: Thu, 23 Apr 2020 01:39:19 GMT  
		Size: 9.6 MB (9613310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adbe3ddd630aa5727b4d0afc72c65882be19ca211d9f9cdd0404c9d4428c568`  
		Last Modified: Thu, 23 Apr 2020 01:40:23 GMT  
		Size: 264.6 MB (264555287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9cc3e6c95b5baabaa0992459a8c906c9690ac798578f3dc8df3036593ea`  
		Last Modified: Thu, 23 Apr 2020 01:39:22 GMT  
		Size: 14.6 MB (14567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

**does not exist** (yet?)
