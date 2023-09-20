## `swift:focal`

```console
$ docker pull swift@sha256:ec1dd07da90598e51fcef47003a7b0d476eb797b3a40d2158f57d4678048a97a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:f0befa183f0842b03e20d24d9eb0271f7543fa3b3da3cfe29411fc16470afb7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **752.0 MB (752006063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74196d8b8532a185d44fd20444ed10415fba7f32e819dde03ad94337a9be235a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 21:11:33 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Mon, 07 Aug 2023 21:11:33 GMT
LABEL description=Docker Container for the Swift programming language
# Mon, 07 Aug 2023 21:13:26 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     unzip     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Mon, 07 Aug 2023 21:13:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 07 Aug 2023 21:13:27 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 20 Sep 2023 03:30:47 GMT
ARG SWIFT_BRANCH=swift-5.9-release
# Wed, 20 Sep 2023 03:30:47 GMT
ARG SWIFT_VERSION=swift-5.9-RELEASE
# Wed, 20 Sep 2023 03:30:47 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 03:30:47 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.9-release SWIFT_VERSION=swift-5.9-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 03:31:32 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 20 Sep 2023 03:31:39 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46de8b29c0de16e7d91e9d591d162b2a09644e4abb441a7538a21faec3e03450`  
		Last Modified: Mon, 07 Aug 2023 21:44:30 GMT  
		Size: 120.5 MB (120476699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc588ced82c782e523bb3ad12841fc8f798ee72d8985a8416635cf1054559a91`  
		Last Modified: Wed, 20 Sep 2023 03:44:39 GMT  
		Size: 602.9 MB (602948494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52733544f2b5b7d1c67c3619c3d64b842a07acd33362fd49dcd7a317a89461f`  
		Last Modified: Wed, 20 Sep 2023 03:43:18 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:focal` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:11ee0043d9d392604224efb1449fcc1d4dbd7e92c685a323be05b6c856ca480b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.0 MB (741989715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8dcfb4463071abd4b56fa2e706f84e95fe9cc929afe1f8b46bcc4bda9cb1635`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 21:10:06 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Mon, 07 Aug 2023 21:10:06 GMT
LABEL description=Docker Container for the Swift programming language
# Mon, 07 Aug 2023 21:11:58 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     unzip     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Mon, 07 Aug 2023 21:12:01 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 07 Aug 2023 21:12:01 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 20 Sep 2023 01:56:12 GMT
ARG SWIFT_BRANCH=swift-5.9-release
# Wed, 20 Sep 2023 01:56:12 GMT
ARG SWIFT_VERSION=swift-5.9-RELEASE
# Wed, 20 Sep 2023 01:56:12 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 01:56:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.9-release SWIFT_VERSION=swift-5.9-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 01:56:55 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 20 Sep 2023 01:57:07 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcfe30a986b00cdd5973550b6bbdb1022db122df650abb1439836565d0ea1d4`  
		Last Modified: Mon, 07 Aug 2023 21:21:39 GMT  
		Size: 117.2 MB (117248346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd5f65608a504384536a5903e24795c6856f3d735f62ff2e19d97d760380c50`  
		Last Modified: Wed, 20 Sep 2023 02:04:20 GMT  
		Size: 597.5 MB (597540580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6404a20a333e4ca0cfe6f84506c8ff7e613da53e12385e808b2a651729c513`  
		Last Modified: Wed, 20 Sep 2023 02:03:21 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
