## `swift:focal`

```console
$ docker pull swift@sha256:15e9bc1f5a816e4769974da32ce813e6134155f56b85be65cf5443060707a044
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:221799ea03dd7384e39a05eeeb851c870f037e31d4c98eb6d70534925fcc8f6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.0 MB (721950622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e6fce3d3123d3e54783f613c4e66eb3c78541bc2609bb93007bc27ec8b0aed`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Thu, 28 Oct 2021 23:48:36 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 28 Oct 2021 23:48:36 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 28 Oct 2021 23:51:10 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Thu, 28 Oct 2021 23:51:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 28 Oct 2021 23:51:11 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 14 Dec 2021 20:30:57 GMT
ARG SWIFT_BRANCH=swift-5.5.2-release
# Tue, 14 Dec 2021 20:30:57 GMT
ARG SWIFT_VERSION=swift-5.5.2-RELEASE
# Tue, 14 Dec 2021 20:30:57 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 14 Dec 2021 20:30:57 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.5.2-release SWIFT_VERSION=swift-5.5.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 14 Dec 2021 20:31:59 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 14 Dec 2021 20:32:04 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7469d4d6c0468fb7965ae7641a3d9598b4801468c56fa1fe337016b823d06c8d`  
		Last Modified: Fri, 29 Oct 2021 00:46:23 GMT  
		Size: 99.0 MB (98990724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377b4d820b60589707ad28381d37be31cb5d5519d0d26c3a427156f99d6ae279`  
		Last Modified: Tue, 14 Dec 2021 20:51:01 GMT  
		Size: 594.4 MB (594392569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b46ab423c80087880cc161ddb94d9bdaa857116b7bbc1f4f3b39ee580e093`  
		Last Modified: Tue, 14 Dec 2021 20:49:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
