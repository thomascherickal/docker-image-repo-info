## `swift:amazonlinux2-slim`

```console
$ docker pull swift@sha256:67f2e9dd06f22fccbc9084f779685a3a5b0b3e1821b21c9e775cfea0c7268e40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:amazonlinux2-slim` - linux; amd64

```console
$ docker pull swift@sha256:2b876d92b890bc5319b93fb837f1c89b91fb5a75ca6e9504ba0c80e8080a9185
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.8 MB (273806477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59b2f2cf5414f52f7c4e3ce7759daf08aefdc716c5d8271e11aaf68e446305c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 23:52:07 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 28 Oct 2021 23:52:07 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 28 Oct 2021 23:53:44 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 28 Oct 2021 23:53:45 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Thu, 28 Oct 2021 23:53:45 GMT
ARG SWIFT_BRANCH=swift-5.5.1-release
# Thu, 28 Oct 2021 23:53:45 GMT
ARG SWIFT_VERSION=swift-5.5.1-RELEASE
# Thu, 28 Oct 2021 23:53:45 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:53:45 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.5.1-release SWIFT_VERSION=swift-5.5.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:54:25 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && yum autoremove -y tar gzip
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb91bddb78f07cc94ddf47b7bd5b3108c579b77a9f01d31458473ca9f25f40e`  
		Last Modified: Fri, 29 Oct 2021 00:49:50 GMT  
		Size: 211.8 MB (211830369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
