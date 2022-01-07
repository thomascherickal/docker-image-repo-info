## `swift:bionic-slim`

```console
$ docker pull swift@sha256:8753a4bba69452a3a81aeeee8f364d425f984af9c946a565a17965f3d662c01f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:bionic-slim` - linux; amd64

```console
$ docker pull swift@sha256:6f5d15bce16dcf70203bafa8955e694cc642ae4a96509b03daaa9e8a552dd4e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139939222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9662b4f6ea2b4146e6b16a86c6fce43099ebeb21c9402e9845c0ccba0ed60ea7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 06:02:06 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 07 Jan 2022 06:02:06 GMT
LABEL Description=Docker Container for the Swift programming language
# Fri, 07 Jan 2022 06:04:43 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 07 Jan 2022 06:04:43 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 07 Jan 2022 06:04:43 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Fri, 07 Jan 2022 06:04:44 GMT
ARG SWIFT_BRANCH=swift-5.5.2-release
# Fri, 07 Jan 2022 06:04:44 GMT
ARG SWIFT_VERSION=swift-5.5.2-RELEASE
# Fri, 07 Jan 2022 06:04:44 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 07 Jan 2022 06:04:44 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.5.2-release SWIFT_VERSION=swift-5.5.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 07 Jan 2022 06:05:22 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a188b6d551e277279c79f17a08ce7252807966aada82a0ad0ee675068dad6a9`  
		Last Modified: Fri, 07 Jan 2022 06:28:53 GMT  
		Size: 20.5 MB (20491853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6691cfe14e3a5d804a5c30bed586caa3ac3f07922c775362e3b6a821ac2a645e`  
		Last Modified: Fri, 07 Jan 2022 06:29:03 GMT  
		Size: 92.7 MB (92742342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
