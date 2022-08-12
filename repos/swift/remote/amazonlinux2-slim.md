## `swift:amazonlinux2-slim`

```console
$ docker pull swift@sha256:c7b5f98c9112dd6adc6cae41421a14a6f3537fcde0147251f542e265f931513c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:amazonlinux2-slim` - linux; amd64

```console
$ docker pull swift@sha256:6d2e416f71d8d0d98f2973da79e3d643fbb8a53a69cfb6e14ffd75dc41da29c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.3 MB (280269067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa535e316776426543f9459b819d9799c225f0b4ae6a7fb286679cf1bece065`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 03:06:36 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 12 Aug 2022 03:06:36 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 12 Aug 2022 03:08:14 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 12 Aug 2022 03:08:14 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 12 Aug 2022 03:08:15 GMT
ARG SWIFT_BRANCH=swift-5.6.2-release
# Fri, 12 Aug 2022 03:08:15 GMT
ARG SWIFT_VERSION=swift-5.6.2-RELEASE
# Fri, 12 Aug 2022 03:08:15 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:08:15 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.6.2-release SWIFT_VERSION=swift-5.6.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:08:51 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && yum autoremove -y tar gzip
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef1c35086bbd99826c6cfb60312fe2fc19b4a350277c17d37c39377917173e9`  
		Last Modified: Fri, 12 Aug 2022 03:24:57 GMT  
		Size: 218.0 MB (217952851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:amazonlinux2-slim` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:ac7aa2c32575b3cf142e2f25169e97327bd3b0c32ebea1a975ffdac8a760c81d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.7 MB (244678547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2d3a23894bd78c9f7c19807bedb82138d268f35ccad1d5eb0798a040a13c63`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:39:26 GMT
ADD file:3ec97c6bec2a8682b0b4088021da97853effeb7dfafb69329cfcb5686c3dee30 in / 
# Fri, 12 Aug 2022 00:39:28 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 03:24:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 12 Aug 2022 03:24:43 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 12 Aug 2022 03:26:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 12 Aug 2022 03:26:11 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 12 Aug 2022 03:26:12 GMT
ARG SWIFT_BRANCH=swift-5.6.2-release
# Fri, 12 Aug 2022 03:26:13 GMT
ARG SWIFT_VERSION=swift-5.6.2-RELEASE
# Fri, 12 Aug 2022 03:26:14 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:26:15 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.6.2-release SWIFT_VERSION=swift-5.6.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:26:46 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && yum autoremove -y tar gzip
```

-	Layers:
	-	`sha256:9f9c648afd7976bdc42d03595d6a1c1c502c47f18abb3f42a9a20b38e7d6e161`  
		Last Modified: Mon, 01 Aug 2022 22:09:01 GMT  
		Size: 63.9 MB (63927916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1406788680bd204edf5785d7e70569573dfc3c110a047e34f5dfc7b18b187881`  
		Last Modified: Fri, 12 Aug 2022 03:28:29 GMT  
		Size: 180.8 MB (180750631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
