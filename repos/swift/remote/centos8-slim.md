## `swift:centos8-slim`

```console
$ docker pull swift@sha256:f62c31f78707c086c25c90b9c0b8177ef51a3c82041a3d57ddc133c2dc3c3f71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:centos8-slim` - linux; amd64

```console
$ docker pull swift@sha256:32556dcd5ff9145bdb713f25067ed8a2e960d847508a1b5cf86d48719a52a8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107121747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95a80100bbaa369472ad41b64798d5f20e847e13af99718d4a38c5ae5d7e78a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:54:53 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Mon, 10 Aug 2020 18:54:53 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 11 Aug 2020 19:36:03 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 11 Aug 2020 19:36:04 GMT
ARG SWIFT_PLATFORM=centos8
# Thu, 17 Sep 2020 22:35:09 GMT
ARG SWIFT_BRANCH=swift-5.3-release
# Thu, 17 Sep 2020 22:35:09 GMT
ARG SWIFT_VERSION=swift-5.3-RELEASE
# Thu, 17 Sep 2020 22:35:09 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Thu, 17 Sep 2020 22:35:09 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos8 SWIFT_BRANCH=swift-5.3-release SWIFT_VERSION=swift-5.3-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Thu, 17 Sep 2020 22:36:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3ef51f8a17be64f6a48b8b550128899a3d75e3afa1685501d6d7dd1fabc7f6`  
		Last Modified: Thu, 17 Sep 2020 22:49:44 GMT  
		Size: 32.3 MB (32253626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
