## `swift:focal`

```console
$ docker pull swift@sha256:4c76988745e8dd63815d56f79d30c9bec05f821f4b7dfb9eaea6f5c8e07627d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:c4bdab91a3fcc08610f1f4a5c3878f15d2d2a9aa9449a6312d7ca3540d2545f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **674.2 MB (674193435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b75db6670642555d4072fed76d336d25339e996d0d5d728290e5ee8d276274`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 03:20:57 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 07 Jun 2022 03:20:57 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 07 Jun 2022 03:22:20 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Tue, 07 Jun 2022 03:22:21 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 07 Jun 2022 03:22:21 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 07 Jun 2022 03:22:21 GMT
ARG SWIFT_BRANCH=swift-5.6.1-release
# Tue, 07 Jun 2022 03:22:21 GMT
ARG SWIFT_VERSION=swift-5.6.1-RELEASE
# Tue, 07 Jun 2022 03:22:21 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 07 Jun 2022 03:22:21 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6.1-release SWIFT_VERSION=swift-5.6.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 07 Jun 2022 03:22:59 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 07 Jun 2022 03:23:05 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37a54a97dd34784b448ab9632d55e68bba48cf91f7f0970f67c0ab2706f76f9`  
		Last Modified: Tue, 07 Jun 2022 03:47:02 GMT  
		Size: 120.1 MB (120098136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f1b78f218c0a292e146bea9155f80135c56fbcea87dc2cffed9e9959852d54`  
		Last Modified: Tue, 07 Jun 2022 03:47:59 GMT  
		Size: 525.5 MB (525522443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dddc9c900fdb14ac149681166501570377dc0ebe5e59b42bf9a633682463a7`  
		Last Modified: Tue, 07 Jun 2022 03:46:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:focal` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:07664875d7fd809337c7862429be512d0a5402e50ee78d8771c02c956acadc45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **639.8 MB (639775367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5e8985ffc56ebf897f9ac928c28332b8974b264cc6191bf0b2c6f044249b14`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:29:03 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 07 Jun 2022 06:29:04 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 07 Jun 2022 06:30:36 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:30:37 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 07 Jun 2022 06:30:37 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 07 Jun 2022 06:30:38 GMT
ARG SWIFT_BRANCH=swift-5.6.1-release
# Tue, 07 Jun 2022 06:30:39 GMT
ARG SWIFT_VERSION=swift-5.6.1-RELEASE
# Tue, 07 Jun 2022 06:30:40 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 07 Jun 2022 06:30:41 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6.1-release SWIFT_VERSION=swift-5.6.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 07 Jun 2022 06:31:15 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 07 Jun 2022 06:31:16 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92635fd0ece424888d31a2b34e692c04006861c50e08ae5d2b423f07a09825b6`  
		Last Modified: Tue, 07 Jun 2022 06:32:46 GMT  
		Size: 116.8 MB (116835842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2606c585bcf8badee4436413bf2e09985b4a48f7391db4a540f2ab9e11d33523`  
		Last Modified: Tue, 07 Jun 2022 06:33:36 GMT  
		Size: 495.7 MB (495748112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a6c85414fed28663c72bca2ba880524b3bba13f29bab4c6f0a380e11cf01b5`  
		Last Modified: Tue, 07 Jun 2022 06:32:28 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
