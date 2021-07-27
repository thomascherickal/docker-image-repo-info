## `swift:focal`

```console
$ docker pull swift@sha256:adae7036dcdc8962b93b1122edfe002a67b50c90117f4ae688925a459a8035b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:5870498bfa6439829439ec0a42330b34d5272704e0dc8dc4fab5f1a86baef0fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **648.4 MB (648394730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5ef0bd73eba4fc08579bb8fb0e4e28d5fafa6f286064632dbee8d4c8099f65`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:25:06 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 27 Jul 2021 02:25:06 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 27 Jul 2021 02:28:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     gnupg2     libc6-dev     libcurl4     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:28:52 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 27 Jul 2021 02:28:52 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 27 Jul 2021 02:28:52 GMT
ARG SWIFT_BRANCH=swift-5.4.2-release
# Tue, 27 Jul 2021 02:28:52 GMT
ARG SWIFT_VERSION=swift-5.4.2-RELEASE
# Tue, 27 Jul 2021 02:28:53 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 27 Jul 2021 02:28:53 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.4.2-release SWIFT_VERSION=swift-5.4.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 27 Jul 2021 02:30:22 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 27 Jul 2021 02:30:27 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331e801caee17f325e0d921d66b84656b9927758006f7d2aaa47c727e6c62c49`  
		Last Modified: Tue, 27 Jul 2021 03:17:03 GMT  
		Size: 99.0 MB (99007918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7443d57efde8c274c70e85b2b44d79af0a409527ad5abb18e609f302d47525da`  
		Last Modified: Tue, 27 Jul 2021 03:17:59 GMT  
		Size: 520.8 MB (520818868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
