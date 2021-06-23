## `haskell:stretch`

```console
$ docker pull haskell@sha256:a36be9ed65a9bbf2668bd66b6b8e8581f13bba537076692d41355a98a295adc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:352a135817e48ec0203ef15ef7ac678d92c1981f0b51fad5f4eb338e7db484f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338604791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6a5773d16c9b362d8e659251336c40585ce3a61634eec192f38ecbf1f4ac04`
-	Default Command: `["ghci"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:08:42 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 06:08:56 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:08:56 GMT
ARG GHC=9.0.1
# Wed, 23 Jun 2021 06:08:56 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Wed, 23 Jun 2021 06:08:56 GMT
ARG CABAL_INSTALL=3.4
# Wed, 23 Jun 2021 06:08:57 GMT
ARG STACK=2.7.1
# Wed, 23 Jun 2021 06:08:57 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Wed, 23 Jun 2021 06:08:57 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Wed, 23 Jun 2021 06:09:56 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:10:07 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.7.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Wed, 23 Jun 2021 06:10:08 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 06:10:08 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b2ed3ac36ac8a16ae55e1f2e60b66f060035ea06ab48052012e9b4ec0982ed`  
		Last Modified: Wed, 23 Jun 2021 06:14:48 GMT  
		Size: 9.6 MB (9587019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616add7f9fd6b1d6d8417585556dc59e0d73d7b3f9628ddc2118c4f369884dc6`  
		Last Modified: Wed, 23 Jun 2021 06:15:50 GMT  
		Size: 265.6 MB (265554412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ff9c6932bb010f23ea856559bd06b6dbdf9cdefb94f11379615650079eb6b`  
		Last Modified: Wed, 23 Jun 2021 06:14:53 GMT  
		Size: 18.1 MB (18083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
