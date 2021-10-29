## `swift:focal`

```console
$ docker pull swift@sha256:d4414ce2257431badb116e75df8f2ec2e86175c07c8cfee1a740c2c7b90a9553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:5c3f82ee647de7b80a70bdfef7882328133436ced00f4b1ff0d93a11c3a52b85
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **720.3 MB (720309725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13428c0ee57e984cd5bf0c6c7973111e67a075c4e89c67b3c91fe5638d3eb235`
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
# Thu, 28 Oct 2021 23:51:11 GMT
ARG SWIFT_BRANCH=swift-5.5.1-release
# Thu, 28 Oct 2021 23:51:12 GMT
ARG SWIFT_VERSION=swift-5.5.1-RELEASE
# Thu, 28 Oct 2021 23:51:12 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:51:12 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.5.1-release SWIFT_VERSION=swift-5.5.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:51:57 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Thu, 28 Oct 2021 23:52:00 GMT
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
	-	`sha256:2f8af14acb373c3511f45c03c15b0d20ff1c08f7c80b80934f39bfd0a14b4005`  
		Last Modified: Fri, 29 Oct 2021 00:47:30 GMT  
		Size: 592.8 MB (592751673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be9536ab090a9224ccedf94a20cb99ca274a0867746b835f22975f78366ada9`  
		Last Modified: Fri, 29 Oct 2021 00:46:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
