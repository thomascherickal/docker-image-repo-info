## `swift:slim`

```console
$ docker pull swift@sha256:9571c179854c16283b1a075f4268bc88b833be50e143a3fba180155ebdf7ffbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:slim` - linux; amd64

```console
$ docker pull swift@sha256:dc3811abfe4c0af445fc9509bcbcf062c640a6bbe49ffea2a64c4cb625ac0b32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139764160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea6f145b5e43c9fcfd2e204fb62d1d0706189b703d1c953c19523fff6fde194`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Thu, 28 Oct 2021 23:39:56 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 28 Oct 2021 23:39:57 GMT
LABEL Description=Docker Container for the Swift programming language
# Thu, 28 Oct 2021 23:46:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Thu, 28 Oct 2021 23:46:51 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 28 Oct 2021 23:46:51 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Thu, 28 Oct 2021 23:46:51 GMT
ARG SWIFT_BRANCH=swift-5.5.1-release
# Thu, 28 Oct 2021 23:46:52 GMT
ARG SWIFT_VERSION=swift-5.5.1-RELEASE
# Thu, 28 Oct 2021 23:46:52 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:46:52 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.5.1-release SWIFT_VERSION=swift-5.5.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 28 Oct 2021 23:47:30 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6a5971fad9eecb542b7651c437da0cef6c0a0a7c86218cf5829c9ad7c7241a`  
		Last Modified: Fri, 29 Oct 2021 00:44:40 GMT  
		Size: 20.5 MB (20490922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7376cd09dd8373b1c493d453b90c4058d7d74a98b903b007e16e1342b184d147`  
		Last Modified: Fri, 29 Oct 2021 00:44:50 GMT  
		Size: 92.6 MB (92568163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
