## `swift:centos7-slim`

```console
$ docker pull swift@sha256:c85baa89ada0ca2606416e6c81f15533c554fabb73fc4f339f0a898863b18485
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:centos7-slim` - linux; amd64

```console
$ docker pull swift@sha256:2842706137bb23e3dadecce577e0688e9d54c968c1ea25f23f3bf8abf48a3384
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113749747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79f599870848484a77bd8278f000d041304d50a01d1a73eccc9052e6c26250c`
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
# Wed, 20 Sep 2023 03:35:42 GMT
ARG SWIFT_BRANCH=swift-5.9-release
# Wed, 20 Sep 2023 03:35:42 GMT
ARG SWIFT_VERSION=swift-5.9-RELEASE
# Wed, 20 Sep 2023 03:35:42 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 03:35:42 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos7 SWIFT_BRANCH=swift-5.9-release SWIFT_VERSION=swift-5.9-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 03:36:15 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1         $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux         $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/libexec/swift/linux     && chmod -R o+r /usr/lib/swift /usr/libexec/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e0a1b070e58df661e5e4b0196a1fd075e74d71c7e209b293297a24b58164a3`  
		Last Modified: Wed, 20 Sep 2023 03:48:33 GMT  
		Size: 37.7 MB (37652590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
