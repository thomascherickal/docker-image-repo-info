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
