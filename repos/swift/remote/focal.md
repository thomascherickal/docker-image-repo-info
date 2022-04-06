## `swift:focal`

```console
$ docker pull swift@sha256:baf8e017cb93a9acf0eac103569192662debc180279312bb072458166060b240
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:9768838769e6c05ab8a17d34144312797480ee7fd22855b116a51dc9f63cc34f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **674.2 MB (674190121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb805adcec99ecebf577aff82dcdac28eb31e7093a326d43acb791e9c353cb5`
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
# Wed, 06 Apr 2022 03:25:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Wed, 06 Apr 2022 03:25:09 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 06 Apr 2022 03:25:09 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 06 Apr 2022 03:25:09 GMT
ARG SWIFT_BRANCH=swift-5.6-release
# Wed, 06 Apr 2022 03:25:09 GMT
ARG SWIFT_VERSION=swift-5.6-RELEASE
# Wed, 06 Apr 2022 03:25:10 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 06 Apr 2022 03:25:10 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6-release SWIFT_VERSION=swift-5.6-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 06 Apr 2022 03:25:48 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 06 Apr 2022 03:25:53 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69ee77541d7de0e825bda77a0fb5391a99ab2aaa386ebaca338dade37dc8203`  
		Last Modified: Wed, 06 Apr 2022 03:49:40 GMT  
		Size: 120.1 MB (120107831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a753d1acd07b6d5542ae12e5fc2afd83c15bf15616694efaea4952677a4e205`  
		Last Modified: Wed, 06 Apr 2022 03:50:37 GMT  
		Size: 525.5 MB (525515768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1aaee8a2fe3cc409a519a298b35a12e4f678909e6aad4c3bea57007a064cc2`  
		Last Modified: Wed, 06 Apr 2022 03:49:17 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:focal` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:521258d3764e7a0bb3073c27a576fc2e0a7278e8999ec0d1b540964d8349e253
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **639.7 MB (639719284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d0d91721fa183e3834979f5c3505b0ca0ca921a01891d430c53f83e94bf787`
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
# Tue, 05 Apr 2022 23:58:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:58:20 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 05 Apr 2022 23:58:21 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 05 Apr 2022 23:58:22 GMT
ARG SWIFT_BRANCH=swift-5.6-release
# Tue, 05 Apr 2022 23:58:23 GMT
ARG SWIFT_VERSION=swift-5.6-RELEASE
# Tue, 05 Apr 2022 23:58:24 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 05 Apr 2022 23:58:25 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6-release SWIFT_VERSION=swift-5.6-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 05 Apr 2022 23:59:05 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 05 Apr 2022 23:59:07 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c518c5ba09a190065d071654df17e89187fcf9834b709d9c67e8c6c323f51c`  
		Last Modified: Wed, 06 Apr 2022 00:00:32 GMT  
		Size: 116.8 MB (116793440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d201b3c8cd7ab0a29de0a8ca9d0af848a74f616878ceb41a6e709af77f1bcc9`  
		Last Modified: Wed, 06 Apr 2022 00:01:22 GMT  
		Size: 495.8 MB (495756247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca130fd16d843e4dd930c9288534097bb368432793475d1b615bcc64dc734781`  
		Last Modified: Wed, 06 Apr 2022 00:00:15 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
