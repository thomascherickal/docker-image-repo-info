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
