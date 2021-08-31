## `swift:bionic`

```console
$ docker pull swift@sha256:4ca92068fded458af995c7667bf497d7ec2f31f0fc7c23be44e7a86e643145da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:bionic` - linux; amd64

```console
$ docker pull swift@sha256:a163b6b7d5eadca5d7e4b1696af00c932f7fd9f64d75fb732d2d4c49fe25ee27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **672.5 MB (672454221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:349cf61d73b60d9ff8b7ae6c8f25748800b29e70807f38afaf33b369d71b9aa0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:12:26 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 31 Aug 2021 05:12:26 GMT
LABEL Description=Docker Container for the Swift programming language
# Tue, 31 Aug 2021 05:14:27 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython3.6     tzdata     git     pkg-config     && rm -r /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:14:28 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 31 Aug 2021 05:14:28 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Tue, 31 Aug 2021 05:14:29 GMT
ARG SWIFT_BRANCH=swift-5.4.2-release
# Tue, 31 Aug 2021 05:14:29 GMT
ARG SWIFT_VERSION=swift-5.4.2-RELEASE
# Tue, 31 Aug 2021 05:14:29 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 31 Aug 2021 05:14:29 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.4.2-release SWIFT_VERSION=swift-5.4.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 31 Aug 2021 05:16:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 31 Aug 2021 05:16:17 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e76d16250a8f57d79710747137a242f611fee2834b1e442c917d91153604c77`  
		Last Modified: Tue, 31 Aug 2021 06:09:52 GMT  
		Size: 124.7 MB (124693120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa829ddb8f6ec516b6df83109944f57a760ed2bb0e67fa85f788d393314b8ec6`  
		Last Modified: Tue, 31 Aug 2021 06:10:48 GMT  
		Size: 521.1 MB (521052590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
