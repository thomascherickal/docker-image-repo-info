## `swift:slim`

```console
$ docker pull swift@sha256:67582b4c361b24065f9795901dae9f2e24e74137bf55f5fc888c7f76b8bf418c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:8d93922edebd17d4a240a848845c781f1f7379adc612b8224ba8271671028545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138989205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9936feb0fe441a5ba64a1585e45df959d2a3912b419f51c3da9afb1d17410ad`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:27:06 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Wed, 14 Sep 2022 00:27:06 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 14 Sep 2022 00:30:06 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:30:06 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 14 Sep 2022 00:30:06 GMT
ARG SWIFT_PLATFORM=ubuntu22.04
# Wed, 14 Sep 2022 00:30:06 GMT
ARG SWIFT_BRANCH=swift-5.7-release
# Wed, 14 Sep 2022 00:30:06 GMT
ARG SWIFT_VERSION=swift-5.7-RELEASE
# Wed, 14 Sep 2022 00:30:06 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:30:06 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu22.04 SWIFT_BRANCH=swift-5.7-release SWIFT_VERSION=swift-5.7-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:30:39 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872c776c1a938e89b5453f371380ac1fcc379303eb6d449180ca8d2859a2638d`  
		Last Modified: Wed, 14 Sep 2022 00:48:51 GMT  
		Size: 19.1 MB (19141935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa5eff73ffb2fd7f13354146c531df0fc4e7065d5aa726b1fbd7e5d33102ef3`  
		Last Modified: Wed, 14 Sep 2022 00:49:01 GMT  
		Size: 89.4 MB (89420564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
