## `haskell:stretch`

```console
$ docker pull haskell@sha256:6bf4df08915e178dbc514032d331c4f715a0337bce30c1845458ae03862388f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `haskell:stretch` - linux; amd64

```console
$ docker pull haskell@sha256:12edd4414e1ab29f28c4fdec6608323ac870c4a57042a27dc9ac37db6d822a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335045249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4f7c75c8cb2561327a394431bae4860c4a193232667443601272d93e901939`
-	Default Command: `["ghci"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:41:04 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 06:41:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gnupg ca-certificates dirmngr &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:41:16 GMT
ARG GHC=9.0.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574
# Sat, 10 Apr 2021 06:41:17 GMT
ARG CABAL_INSTALL=3.4
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK=2.5.1
# Sat, 10 Apr 2021 06:41:17 GMT
ARG STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442
# Sat, 10 Apr 2021 06:41:18 GMT
ARG STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
# Sat, 10 Apr 2021 06:42:08 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys ${DEBIAN_KEY} &&     gpg --batch --armor --export ${DEBIAN_KEY} > /etc/apt/trusted.gpg.d/haskell.org.gpg.asc &&     gpgconf --kill all &&     echo 'deb http://downloads.haskell.org/debian stretch main' > /etc/apt/sources.list.d/ghc.list &&     apt-get update &&     apt-get install -y --no-install-recommends         cabal-install-${CABAL_INSTALL}         curl         g++         ghc-${GHC}         git         libsqlite3-dev         libtinfo-dev         make         netbase         openssh-client         xz-utils         zlib1g-dev &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:42:15 GMT
# ARGS: CABAL_INSTALL=3.4 DEBIAN_KEY=427CB69AAC9D00F2A43CAF1CBA3CBA3FFE22B574 GHC=9.0.1 STACK=2.5.1 STACK_KEY=C5705533DA4F78D8664B5DC0575159689BEFB442 STACK_RELEASE_KEY=2C6A674E85EE3FB896AFC9B965101FF31C5C154D
RUN export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_KEY} &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys ${STACK_RELEASE_KEY} &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz -o stack.tar.gz &&     curl -fSL https://github.com/commercialhaskell/stack/releases/download/v${STACK}/stack-${STACK}-linux-x86_64.tar.gz.asc -o stack.tar.gz.asc &&     gpg --batch --trusted-key 0x575159689BEFB442 --verify stack.tar.gz.asc stack.tar.gz &&     tar -xf stack.tar.gz -C /usr/local/bin --strip-components=1 &&     /usr/local/bin/stack config set system-ghc --global true &&     /usr/local/bin/stack config set install-ghc --global false &&     rm -rf "$GNUPGHOME" /var/lib/apt/lists/* /stack.tar.gz.asc /stack.tar.gz
# Sat, 10 Apr 2021 06:42:16 GMT
ENV PATH=/root/.cabal/bin:/root/.local/bin:/opt/cabal/3.4/bin:/opt/ghc/9.0.1/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:42:16 GMT
CMD ["ghci"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da365b0f8316fd12a58e64e937a373e81d5d2f8c9fe169a1a25b4b1d97460227`  
		Last Modified: Sat, 10 Apr 2021 06:47:13 GMT  
		Size: 9.6 MB (9586956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb1230c1469292c284b197e9534fd3a886f4a2737e6c1e59e094c7e7f905e7`  
		Last Modified: Sat, 10 Apr 2021 06:48:17 GMT  
		Size: 265.5 MB (265515583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a5806c2c0e0a050544356c0ad0962507e7f90b6582cc7ff8451292d0ddc8e`  
		Last Modified: Sat, 10 Apr 2021 06:47:17 GMT  
		Size: 14.6 MB (14562673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
