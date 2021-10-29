## `swift:focal-slim`

```console
$ docker pull swift@sha256:e751be222dc38e7a60824642f939092f1686be21caa73ffa2755fe19263e3546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:ecf3fdd5f7afa5477ad7323685abdeed7ea21a67799d8af2deaaa6ea19a7c54e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (142984991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863840fc91aaa2c92f1b078783630f3457e0d7bd52f9d4711ea2b4cf33fb3ec`
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
# Thu, 28 Oct 2021 23:49:04 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Thu, 28 Oct 2021 23:49:05 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 28 Oct 2021 23:49:05 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Thu, 28 Oct 2021 23:49:05 GMT
ARG SWIFT_BRANCH=swift-5.5.1-release
# Thu, 28 Oct 2021 23:49:05 GMT
ARG SWIFT_VERSION=swift-5.5.1-RELEASE
# Thu, 28 Oct 2021 23:49:05 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:49:06 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.5.1-release SWIFT_VERSION=swift-5.5.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:49:59 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbba385b5299cafec1cd2c4ba071ab30e08d1f3b37a9e12e89fbab0d75acc196`  
		Last Modified: Fri, 29 Oct 2021 00:45:40 GMT  
		Size: 22.3 MB (22254629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c22ef5360f597fdc770b94b9b1ef7c210439bcff61bf800a09c31372a13253d`  
		Last Modified: Fri, 29 Oct 2021 00:45:50 GMT  
		Size: 92.2 MB (92163261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
