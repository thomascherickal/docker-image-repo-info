## `swift:centos7-slim`

```console
$ docker pull swift@sha256:54ae60d24d60d20df5c6e896358fbdf47eaf9cd8d4a2647a6af640a455cdc418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:centos7-slim` - linux; amd64

```console
$ docker pull swift@sha256:477bf9a5566a4c5f3f42817dd4aa4fd1db9eb316ac2fb0dba51d372683a7d386
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159868689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7defceabd127a87495cff91d1ed56f1d3bdfd63e9aa9571ee287e50ca7e6b1ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 23:56:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 28 Oct 2021 23:56:50 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 28 Oct 2021 23:58:58 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 28 Oct 2021 23:58:58 GMT
ARG SWIFT_PLATFORM=centos7
# Thu, 16 Jun 2022 17:26:51 GMT
ARG SWIFT_BRANCH=swift-5.6.2-release
# Thu, 16 Jun 2022 17:26:51 GMT
ARG SWIFT_VERSION=swift-5.6.2-RELEASE
# Thu, 16 Jun 2022 17:26:51 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 16 Jun 2022 17:26:51 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos7 SWIFT_BRANCH=swift-5.6.2-release SWIFT_VERSION=swift-5.6.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 16 Jun 2022 17:27:14 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ccd4be3b329a3ad30bd8fcfa18cb4ca40a422d9ff3e31f99c4feca1003bb7`  
		Last Modified: Thu, 16 Jun 2022 17:43:17 GMT  
		Size: 83.8 MB (83771532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
