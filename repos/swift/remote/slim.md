## `swift:slim`

```console
$ docker pull swift@sha256:8168db80f915d69500fe7da598c00338dc7e371d21a034a7ae0a619eb1be8f07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:8b661a6ec4bb96f7ecdafe662ffe42e280b5ade9631a73331048fcd9b6f24c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (139004148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6695608aa19579ce99c1cc1c5a0712c210dc8a8023a08b02f36e760b51d8a966`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 05:47:19 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 02 Mar 2023 05:47:19 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 02 Mar 2023 05:49:35 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Thu, 02 Mar 2023 05:49:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 02 Mar 2023 05:49:35 GMT
ARG SWIFT_PLATFORM=ubuntu22.04
# Thu, 02 Mar 2023 05:49:35 GMT
ARG SWIFT_BRANCH=swift-5.7.3-release
# Thu, 02 Mar 2023 05:49:35 GMT
ARG SWIFT_VERSION=swift-5.7.3-RELEASE
# Thu, 02 Mar 2023 05:49:36 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 02 Mar 2023 05:49:36 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu22.04 SWIFT_BRANCH=swift-5.7.3-release SWIFT_VERSION=swift-5.7.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 02 Mar 2023 05:50:02 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7800eccca4936d34339975e902a8ee33ce01d7540f8d404350fa7a71e997d3`  
		Last Modified: Thu, 02 Mar 2023 06:24:12 GMT  
		Size: 19.1 MB (19127317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1817a1a5a4dc3f9a42eb9a374421aaf4ac631f711d48102173670eeb687225f2`  
		Last Modified: Thu, 02 Mar 2023 06:24:21 GMT  
		Size: 89.4 MB (89446829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:slim` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:d19af50b770e8b8b659f3ebb03a40c68a8e2188d38d8e6ddba783f1bdadcf283
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135676883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:887b3522d03998e479fbf0bd937a9aae56bd5df924fed3a07b304901dd353ad9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:27 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 02 Mar 2023 04:14:27 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 02 Mar 2023 04:16:11 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:16:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 02 Mar 2023 04:16:11 GMT
ARG SWIFT_PLATFORM=ubuntu22.04
# Thu, 02 Mar 2023 04:16:11 GMT
ARG SWIFT_BRANCH=swift-5.7.3-release
# Thu, 02 Mar 2023 04:16:11 GMT
ARG SWIFT_VERSION=swift-5.7.3-RELEASE
# Thu, 02 Mar 2023 04:16:11 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 02 Mar 2023 04:16:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu22.04 SWIFT_BRANCH=swift-5.7.3-release SWIFT_VERSION=swift-5.7.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 02 Mar 2023 04:16:36 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1360d3ead6d272d6c040c61905f0a136a8bf6ebec9e93f387650716bdf099927`  
		Last Modified: Thu, 02 Mar 2023 04:23:51 GMT  
		Size: 19.0 MB (19012210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbf446f1fde49225d3222956c3ee83533f0bb48aff8ccfee313404f60a66f96`  
		Last Modified: Thu, 02 Mar 2023 04:23:57 GMT  
		Size: 88.3 MB (88276751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
