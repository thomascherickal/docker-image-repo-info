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
