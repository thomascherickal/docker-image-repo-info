## `swift:focal-slim`

```console
$ docker pull swift@sha256:885b3097c99892df9f7493245a156e393de1b4506c1d974245fc151e0e8c2045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:0374f9dfcc05b830bd1ab689a62e80ddd43a18fa897e6f2d1a8a48dd4b288d59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135119698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae6019c2bdfd535b21cd8a422750a7010f491649adfb1756f46db4bd53a0343f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 03:22:39 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Wed, 06 Apr 2022 03:22:39 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 06 Apr 2022 03:23:14 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 06 Apr 2022 03:23:15 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 06 Apr 2022 03:23:15 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 06 Apr 2022 03:23:15 GMT
ARG SWIFT_BRANCH=swift-5.6-release
# Wed, 06 Apr 2022 03:23:15 GMT
ARG SWIFT_VERSION=swift-5.6-RELEASE
# Wed, 06 Apr 2022 03:23:15 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 06 Apr 2022 03:23:15 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6-release SWIFT_VERSION=swift-5.6-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 06 Apr 2022 03:23:52 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59ad1614b991560898b9d47f9d15d1d08f74f3a5b92869633ab1d718d2884eb`  
		Last Modified: Wed, 06 Apr 2022 03:48:57 GMT  
		Size: 22.2 MB (22248710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4d0a17a80cea15aa350ec3aaec9f8a75ceeb3ecfcc2d9f0f672a7ecf44d1af`  
		Last Modified: Wed, 06 Apr 2022 03:49:05 GMT  
		Size: 84.3 MB (84304696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:focal-slim` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:0ef97ea78064a2e23b66b407771b5f0986cf443f673ce909fba6de43db205c32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129462095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d35f2b84a52d785f4498e90760c2430446ff7bfbb41652fa77c8e69a7c5af6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:56:47 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 05 Apr 2022 23:56:48 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 05 Apr 2022 23:57:03 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:57:04 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 05 Apr 2022 23:57:05 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 05 Apr 2022 23:57:06 GMT
ARG SWIFT_BRANCH=swift-5.6-release
# Tue, 05 Apr 2022 23:57:07 GMT
ARG SWIFT_VERSION=swift-5.6-RELEASE
# Tue, 05 Apr 2022 23:57:08 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 05 Apr 2022 23:57:09 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6-release SWIFT_VERSION=swift-5.6-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 05 Apr 2022 23:57:39 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f224cccd7a1449b119e7e7f70a3793fb787cb5513eed1a920b6af7b8e6a46cbc`  
		Last Modified: Tue, 05 Apr 2022 23:59:52 GMT  
		Size: 22.0 MB (22030913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22168befd468f221033d2023e8ccfa501fa9498edca904c8b3acc29afdbab2cd`  
		Last Modified: Wed, 06 Apr 2022 00:00:00 GMT  
		Size: 80.3 MB (80261789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
