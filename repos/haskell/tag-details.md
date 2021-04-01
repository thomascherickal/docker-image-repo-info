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
$ docker pull haskell@sha256:bd0d1f229f563f731969e2980d49c20f5253de267ae6d565f1329c3fe18ec82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8` - linux; amd64

```console
$ docker pull haskell@sha256:66a9e2353d1f36509b686cf148b00961e1a7c2550ab071269ba8c12782c4108d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357610782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb9e32509df3a43b014a32f7ab9797b5af01ad9019274a46aa0a9476cc8b22e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:45 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:21:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:21:46 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:22:42 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:22:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:22:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f31d1721ba573ebc90bb13559e1557963cb522009c48608a5c3c84441a0f2`  
		Last Modified: Thu, 01 Apr 2021 02:35:19 GMT  
		Size: 278.8 MB (278762053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065feecd6c412edf07309a1bd8f27fd61663b7b7ebf89449699f0ccc89cffee8`  
		Last Modified: Thu, 01 Apr 2021 02:33:59 GMT  
		Size: 14.6 MB (14562641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-buster`

```console
$ docker pull haskell@sha256:bd0d1f229f563f731969e2980d49c20f5253de267ae6d565f1329c3fe18ec82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:66a9e2353d1f36509b686cf148b00961e1a7c2550ab071269ba8c12782c4108d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357610782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb9e32509df3a43b014a32f7ab9797b5af01ad9019274a46aa0a9476cc8b22e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:45 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:21:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:21:46 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:22:42 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:22:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:22:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f31d1721ba573ebc90bb13559e1557963cb522009c48608a5c3c84441a0f2`  
		Last Modified: Thu, 01 Apr 2021 02:35:19 GMT  
		Size: 278.8 MB (278762053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065feecd6c412edf07309a1bd8f27fd61663b7b7ebf89449699f0ccc89cffee8`  
		Last Modified: Thu, 01 Apr 2021 02:33:59 GMT  
		Size: 14.6 MB (14562641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8-stretch`

```console
$ docker pull haskell@sha256:512c95e89fdb2a50969996440902500db54521364b09cbcd1bdad1f221b54f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:cd74e59c8ae6ef1f41e6917def0f1b4a373c532122f47be879eae7698c39e275
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337072336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0228af50d53456a1982b4015d95d239e83700c30993214bb7135180fd06a6e6a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:57 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:22:57 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:22:57 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:22:57 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:22:58 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:22:58 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:23:41 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:23:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:23:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:23:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faf48e1446b0566d3982e3ca6355ce0944822a4931d9f27c78b326d9706843b`  
		Last Modified: Thu, 01 Apr 2021 02:37:06 GMT  
		Size: 267.5 MB (267542660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b544ad0364285a3351e1fd11d24bc545a754b7dde503ae41134dd6318fdbe`  
		Last Modified: Thu, 01 Apr 2021 02:35:49 GMT  
		Size: 14.6 MB (14562678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10`

```console
$ docker pull haskell@sha256:bd0d1f229f563f731969e2980d49c20f5253de267ae6d565f1329c3fe18ec82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10` - linux; amd64

```console
$ docker pull haskell@sha256:66a9e2353d1f36509b686cf148b00961e1a7c2550ab071269ba8c12782c4108d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357610782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb9e32509df3a43b014a32f7ab9797b5af01ad9019274a46aa0a9476cc8b22e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:45 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:21:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:21:46 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:22:42 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:22:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:22:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f31d1721ba573ebc90bb13559e1557963cb522009c48608a5c3c84441a0f2`  
		Last Modified: Thu, 01 Apr 2021 02:35:19 GMT  
		Size: 278.8 MB (278762053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065feecd6c412edf07309a1bd8f27fd61663b7b7ebf89449699f0ccc89cffee8`  
		Last Modified: Thu, 01 Apr 2021 02:33:59 GMT  
		Size: 14.6 MB (14562641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-buster`

```console
$ docker pull haskell@sha256:bd0d1f229f563f731969e2980d49c20f5253de267ae6d565f1329c3fe18ec82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-buster` - linux; amd64

```console
$ docker pull haskell@sha256:66a9e2353d1f36509b686cf148b00961e1a7c2550ab071269ba8c12782c4108d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357610782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb9e32509df3a43b014a32f7ab9797b5af01ad9019274a46aa0a9476cc8b22e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:45 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:21:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:21:46 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:22:42 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:22:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:22:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f31d1721ba573ebc90bb13559e1557963cb522009c48608a5c3c84441a0f2`  
		Last Modified: Thu, 01 Apr 2021 02:35:19 GMT  
		Size: 278.8 MB (278762053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065feecd6c412edf07309a1bd8f27fd61663b7b7ebf89449699f0ccc89cffee8`  
		Last Modified: Thu, 01 Apr 2021 02:33:59 GMT  
		Size: 14.6 MB (14562641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10-stretch`

```console
$ docker pull haskell@sha256:512c95e89fdb2a50969996440902500db54521364b09cbcd1bdad1f221b54f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:cd74e59c8ae6ef1f41e6917def0f1b4a373c532122f47be879eae7698c39e275
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337072336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0228af50d53456a1982b4015d95d239e83700c30993214bb7135180fd06a6e6a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:57 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:22:57 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:22:57 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:22:57 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:22:58 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:22:58 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:23:41 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:23:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:23:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:23:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faf48e1446b0566d3982e3ca6355ce0944822a4931d9f27c78b326d9706843b`  
		Last Modified: Thu, 01 Apr 2021 02:37:06 GMT  
		Size: 267.5 MB (267542660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b544ad0364285a3351e1fd11d24bc545a754b7dde503ae41134dd6318fdbe`  
		Last Modified: Thu, 01 Apr 2021 02:35:49 GMT  
		Size: 14.6 MB (14562678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4`

```console
$ docker pull haskell@sha256:bd0d1f229f563f731969e2980d49c20f5253de267ae6d565f1329c3fe18ec82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.4` - linux; amd64

```console
$ docker pull haskell@sha256:66a9e2353d1f36509b686cf148b00961e1a7c2550ab071269ba8c12782c4108d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357610782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb9e32509df3a43b014a32f7ab9797b5af01ad9019274a46aa0a9476cc8b22e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:45 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:21:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:21:46 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:22:42 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:22:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:22:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f31d1721ba573ebc90bb13559e1557963cb522009c48608a5c3c84441a0f2`  
		Last Modified: Thu, 01 Apr 2021 02:35:19 GMT  
		Size: 278.8 MB (278762053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065feecd6c412edf07309a1bd8f27fd61663b7b7ebf89449699f0ccc89cffee8`  
		Last Modified: Thu, 01 Apr 2021 02:33:59 GMT  
		Size: 14.6 MB (14562641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4-buster`

```console
$ docker pull haskell@sha256:bd0d1f229f563f731969e2980d49c20f5253de267ae6d565f1329c3fe18ec82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.4-buster` - linux; amd64

```console
$ docker pull haskell@sha256:66a9e2353d1f36509b686cf148b00961e1a7c2550ab071269ba8c12782c4108d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357610782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb9e32509df3a43b014a32f7ab9797b5af01ad9019274a46aa0a9476cc8b22e`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:45 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:21:45 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:21:46 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:21:46 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:22:42 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:22:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:22:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f31d1721ba573ebc90bb13559e1557963cb522009c48608a5c3c84441a0f2`  
		Last Modified: Thu, 01 Apr 2021 02:35:19 GMT  
		Size: 278.8 MB (278762053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065feecd6c412edf07309a1bd8f27fd61663b7b7ebf89449699f0ccc89cffee8`  
		Last Modified: Thu, 01 Apr 2021 02:33:59 GMT  
		Size: 14.6 MB (14562641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:8.10.4-stretch`

```console
$ docker pull haskell@sha256:512c95e89fdb2a50969996440902500db54521364b09cbcd1bdad1f221b54f51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8.10.4-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:cd74e59c8ae6ef1f41e6917def0f1b4a373c532122f47be879eae7698c39e275
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.1 MB (337072336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0228af50d53456a1982b4015d95d239e83700c30993214bb7135180fd06a6e6a`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:22:57 GMT
ARG GHC=8.10.4
# Thu, 01 Apr 2021 02:22:57 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:22:57 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:22:57 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:22:58 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:22:58 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:23:41 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:23:48 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.4 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:23:48 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/8.10.4/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:23:48 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faf48e1446b0566d3982e3ca6355ce0944822a4931d9f27c78b326d9706843b`  
		Last Modified: Thu, 01 Apr 2021 02:37:06 GMT  
		Size: 267.5 MB (267542660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b544ad0364285a3351e1fd11d24bc545a754b7dde503ae41134dd6318fdbe`  
		Last Modified: Thu, 01 Apr 2021 02:35:49 GMT  
		Size: 14.6 MB (14562678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-buster`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9-buster` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9-stretch`

```console
$ docker pull haskell@sha256:62f4227f3675051fa80ca639a9666a3b46a6808681a25039f985e8639bbc1f84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:a96d3b733a0c4a499ce70d1fdb7a8cf4f03c69cf96bbab3a054c2d399357931b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c513ee4bc5e85e5415299adea71ef1a0e6fe67dc704cf51bde5f275f274f4b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:19 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:20:19 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:20:19 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:21:23 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:30 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:21:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:21:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26835674601ca69c22ed8a95d9440f621566338b266ed6e9fec76bf644eda354`  
		Last Modified: Thu, 01 Apr 2021 02:33:32 GMT  
		Size: 265.5 MB (265515551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f886eca01cf323c575ae9701c1a7f5187a1ca9cf2ba0ccc9b86af9e975a2ff`  
		Last Modified: Thu, 01 Apr 2021 02:32:17 GMT  
		Size: 14.6 MB (14562697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-buster`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0-buster` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0-stretch`

```console
$ docker pull haskell@sha256:62f4227f3675051fa80ca639a9666a3b46a6808681a25039f985e8639bbc1f84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:a96d3b733a0c4a499ce70d1fdb7a8cf4f03c69cf96bbab3a054c2d399357931b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c513ee4bc5e85e5415299adea71ef1a0e6fe67dc704cf51bde5f275f274f4b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:19 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:20:19 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:20:19 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:21:23 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:30 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:21:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:21:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26835674601ca69c22ed8a95d9440f621566338b266ed6e9fec76bf644eda354`  
		Last Modified: Thu, 01 Apr 2021 02:33:32 GMT  
		Size: 265.5 MB (265515551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f886eca01cf323c575ae9701c1a7f5187a1ca9cf2ba0ccc9b86af9e975a2ff`  
		Last Modified: Thu, 01 Apr 2021 02:32:17 GMT  
		Size: 14.6 MB (14562697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0.1` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-buster`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0.1-buster` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:9.0.1-stretch`

```console
$ docker pull haskell@sha256:62f4227f3675051fa80ca639a9666a3b46a6808681a25039f985e8639bbc1f84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:9.0.1-stretch` - linux; amd64

```console
$ docker pull haskell@sha256:a96d3b733a0c4a499ce70d1fdb7a8cf4f03c69cf96bbab3a054c2d399357931b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c513ee4bc5e85e5415299adea71ef1a0e6fe67dc704cf51bde5f275f274f4b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:19 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:20:19 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:20:19 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:21:23 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:30 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:21:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:21:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26835674601ca69c22ed8a95d9440f621566338b266ed6e9fec76bf644eda354`  
		Last Modified: Thu, 01 Apr 2021 02:33:32 GMT  
		Size: 265.5 MB (265515551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f886eca01cf323c575ae9701c1a7f5187a1ca9cf2ba0ccc9b86af9e975a2ff`  
		Last Modified: Thu, 01 Apr 2021 02:32:17 GMT  
		Size: 14.6 MB (14562697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:buster`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:buster` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:latest`

```console
$ docker pull haskell@sha256:5ad5c100290da2567b7168fed52ef30bd2f7bde32f4a39e1fce9cfbc2effd9a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:latest` - linux; amd64

```console
$ docker pull haskell@sha256:3dd67b12bd278328f99281b3c2b10640864fdd36c1a6bad74848b40836ef16d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.6 MB (355566338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d565300917ceb1a36b23e8fba8a4250bc45113b1d3be124a4c720c0b2595d10`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:02:56 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:03:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:18:52 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:18:53 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:18:53 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:18:53 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:18:54 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:19:54 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:03 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:20:03 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:20:03 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad260544cf2fa38f837713f9084f14a108fd6885600daacbb694d8dbca3c3e5`  
		Last Modified: Wed, 31 Mar 2021 04:09:11 GMT  
		Size: 13.9 MB (13853246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f53b369fde7f285157711ec259978e6ea16dcedf6708f849297302c361d9e9`  
		Last Modified: Thu, 01 Apr 2021 02:31:40 GMT  
		Size: 276.7 MB (276717608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc14cea54670950feca5418b3c7d9452b4e4444b8ccb784e70c536a92844fcd4`  
		Last Modified: Thu, 01 Apr 2021 02:30:25 GMT  
		Size: 14.6 MB (14562642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haskell:stretch`

```console
$ docker pull haskell@sha256:62f4227f3675051fa80ca639a9666a3b46a6808681a25039f985e8639bbc1f84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:a96d3b733a0c4a499ce70d1fdb7a8cf4f03c69cf96bbab3a054c2d399357931b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c513ee4bc5e85e5415299adea71ef1a0e6fe67dc704cf51bde5f275f274f4b`
-	Default Command: `["ghci"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 04:04:22 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 04:04:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:20:19 GMT
ARG GHC=9.0.1
# Thu, 01 Apr 2021 02:20:19 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Thu, 01 Apr 2021 02:20:19 GMT
ARG CABAL_INSTALL=3.4
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK=2.5.1
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Thu, 01 Apr 2021 02:20:20 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Thu, 01 Apr 2021 02:21:23 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Thu, 01 Apr 2021 02:21:30 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Thu, 01 Apr 2021 02:21:31 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 02:21:31 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ef5fea8336e0637a1ef8a56a63e7bbe64e641b77a22258574bb569d25189b4`  
		Last Modified: Wed, 31 Mar 2021 04:10:51 GMT  
		Size: 9.6 MB (9587049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26835674601ca69c22ed8a95d9440f621566338b266ed6e9fec76bf644eda354`  
		Last Modified: Thu, 01 Apr 2021 02:33:32 GMT  
		Size: 265.5 MB (265515551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f886eca01cf323c575ae9701c1a7f5187a1ca9cf2ba0ccc9b86af9e975a2ff`  
		Last Modified: Thu, 01 Apr 2021 02:32:17 GMT  
		Size: 14.6 MB (14562697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
