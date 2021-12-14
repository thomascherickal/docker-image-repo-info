## `swift:amazonlinux2-slim`

```console
$ docker pull swift@sha256:fbcf0bcc7c2bf47d9dc5b18a111b60847b72a60124e77ba4613a2642c9489774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:amazonlinux2-slim` - linux; amd64

```console
$ docker pull swift@sha256:f4cba0e8ddd824c1c8c325cc3daf75331716e1f0c1805ad195b27510bebbe7fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.6 MB (277607510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19d99304e60a474657af95f9b9340e6d239bf2ba96a98a44ec7df17da71d5a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:03 GMT
ADD file:4eca58da351122eac20ffd87e3af2c0313089cb81650bdd4c2ef95a556fb842a in / 
# Thu, 02 Dec 2021 23:20:04 GMT
CMD ["/bin/bash"]
# Fri, 03 Dec 2021 21:28:06 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 03 Dec 2021 21:28:07 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 03 Dec 2021 21:29:59 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 03 Dec 2021 21:29:59 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Tue, 14 Dec 2021 20:33:15 GMT
ARG SWIFT_BRANCH=swift-5.5.2-release
# Tue, 14 Dec 2021 20:33:15 GMT
ARG SWIFT_VERSION=swift-5.5.2-RELEASE
# Tue, 14 Dec 2021 20:33:15 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 14 Dec 2021 20:33:16 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.5.2-release SWIFT_VERSION=swift-5.5.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 14 Dec 2021 20:33:57 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && yum autoremove -y tar gzip
```

-	Layers:
	-	`sha256:8b8a142162d22658bdf0283afcd00a9dd216c6637943ffe5f2ba53c4e3da0bd9`  
		Last Modified: Thu, 02 Dec 2021 06:01:08 GMT  
		Size: 62.1 MB (62090346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffb0978540098a798b40e89bacda0e39a9bdebd5b505d942a26f4dfec481840`  
		Last Modified: Tue, 14 Dec 2021 20:53:23 GMT  
		Size: 215.5 MB (215517164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
