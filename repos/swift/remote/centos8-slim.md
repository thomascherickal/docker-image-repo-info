## `swift:centos8-slim`

```console
$ docker pull swift@sha256:a8b9a535ebb7af70d12d8197b1795ee86dc5ed4e6863cfbc83b3a8c7c1312588
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:centos8-slim` - linux; amd64

```console
$ docker pull swift@sha256:0ed52a819f50a2fb25e8f5c6fae8f8548fd2aafabf89c7a13f71802ae08a0b74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.5 MB (175517595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aabcaec86805682c40f274fe7460151b47569cdd0a1ab578c84ed78aa9ce613`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 23:54:32 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 28 Oct 2021 23:54:33 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 28 Oct 2021 23:56:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 28 Oct 2021 23:56:10 GMT
ARG SWIFT_PLATFORM=centos8
# Tue, 14 Dec 2021 20:35:12 GMT
ARG SWIFT_BRANCH=swift-5.5.2-release
# Tue, 14 Dec 2021 20:35:12 GMT
ARG SWIFT_VERSION=swift-5.5.2-RELEASE
# Tue, 14 Dec 2021 20:35:12 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 14 Dec 2021 20:35:13 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos8 SWIFT_BRANCH=swift-5.5.2-release SWIFT_VERSION=swift-5.5.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 14 Dec 2021 20:35:56 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a11f93714a24dd69295521b6e5690b785a81c230fd05ae72833e26c81bcab`  
		Last Modified: Tue, 14 Dec 2021 20:55:32 GMT  
		Size: 92.0 MB (91999509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
