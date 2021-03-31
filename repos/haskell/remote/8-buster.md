## `haskell:8-buster`

```console
$ docker pull haskell@sha256:4ea2d7f793ce42a3419788f89197a8977def3777b59a8512c6f873cea1124247
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:8-buster` - linux; amd64

```console
$ docker pull haskell@sha256:990f4ee34d3e1f39d008db97b4a811819ca21aca562b888fef40eee9f9c067fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.3 MB (357251085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2933bb0406994b54343a8ff9a15b4092895dd2d591f12218e76d6ce9586dbd1d`
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
# Wed, 31 Mar 2021 04:03:05 GMT
ARG GHC=8.10.2
# Wed, 31 Mar 2021 04:03:06 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Wed, 31 Mar 2021 04:03:06 GMT
ARG CABAL_INSTALL=3.2
# Wed, 31 Mar 2021 04:03:06 GMT
ARG STACK=2.5.1
# Wed, 31 Mar 2021 04:03:06 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 31 Mar 2021 04:03:06 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Wed, 31 Mar 2021 04:03:59 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian buster main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Wed, 31 Mar 2021 04:04:08 GMT
# ARGS: CABAL_INSTALL=3.2 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=8.10.2 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Wed, 31 Mar 2021 04:04:09 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.2/bin:/opt/ghc/8.10.2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 04:04:09 GMT
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
	-	`sha256:86ef45fba480843a1ed254014ee7fb353193271422c2d7030e83693a642f09b1`  
		Last Modified: Wed, 31 Mar 2021 04:10:14 GMT  
		Size: 278.4 MB (278402349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ec6fab7c010afa50630de5942f3661f94764dca1c31583315237105fc5c6fc`  
		Last Modified: Wed, 31 Mar 2021 04:09:14 GMT  
		Size: 14.6 MB (14562648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
