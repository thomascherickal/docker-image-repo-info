## `swift:focal-slim`

```console
$ docker pull swift@sha256:454e96a9d414fada95e623a07ba34163e2d60b35ce13f397cd19fcf421b5f97b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:87e38c1f673a6a6421741114154657bf8a6d3ab5fe11f39404482df2e5ffa2e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90356862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e5a38c9dc7840e20cdf72ab12a0205b53efbf75018109f957b4a7d535153e9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 05:23:41 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Tue, 31 Aug 2021 05:23:41 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 31 Aug 2021 05:23:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:23:52 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 31 Aug 2021 05:23:52 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Tue, 31 Aug 2021 05:23:52 GMT
ARG SWIFT_BRANCH=swift-5.4.2-release
# Tue, 31 Aug 2021 05:23:52 GMT
ARG SWIFT_VERSION=swift-5.4.2-RELEASE
# Tue, 31 Aug 2021 05:23:53 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 31 Aug 2021 05:23:53 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.4.2-release SWIFT_VERSION=swift-5.4.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Tue, 31 Aug 2021 05:25:18 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc82f57ae84046abb4a72cca7fd12355a13431d6dd32b5891f94b39c02815d4`  
		Last Modified: Tue, 31 Aug 2021 06:13:29 GMT  
		Size: 22.3 MB (22252794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729239b22c1542c1333e6887fadf6ed0a11d2aa1b70bfa71af8b9a9f17cccb29`  
		Last Modified: Tue, 31 Aug 2021 06:13:32 GMT  
		Size: 39.5 MB (39533994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
