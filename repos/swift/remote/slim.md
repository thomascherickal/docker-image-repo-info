## `swift:slim`

```console
$ docker pull swift@sha256:84587a5b6568f6daf60cb7fb63ab0983b2be61b0d0bb8be93d7442e02721a88b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:db2e5b07db1a784c1b99b58ac16180a5050220366927607e0e1241b83e8233e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131708301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfdf2e88cb342af9460695076646e9d7b70d8026f9e8d973466992cee39ce38`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:55:44 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 06 Sep 2022 20:55:44 GMT
LABEL Description=Docker Container for the Swift programming language
# Tue, 06 Sep 2022 20:57:38 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:57:38 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 06 Sep 2022 20:57:38 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Mon, 12 Sep 2022 18:22:43 GMT
ARG SWIFT_BRANCH=swift-5.6.3-release
# Mon, 12 Sep 2022 18:22:43 GMT
ARG SWIFT_VERSION=swift-5.6.3-RELEASE
# Mon, 12 Sep 2022 18:22:44 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Sep 2022 18:22:44 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.6.3-release SWIFT_VERSION=swift-5.6.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Sep 2022 18:23:20 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0525ecb3dfd004198ef23af5b3341058dd014ee73957a05f9cc4106e95cad0ee`  
		Last Modified: Tue, 06 Sep 2022 21:16:04 GMT  
		Size: 20.5 MB (20479391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebcc65e6616eccebedc13d7a1b534c50e1b30f2fd8c32ff35abfba9c7ea0e4b`  
		Last Modified: Mon, 12 Sep 2022 18:39:40 GMT  
		Size: 84.5 MB (84518077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
