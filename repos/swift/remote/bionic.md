## `swift:bionic`

```console
$ docker pull swift@sha256:1868ff4e02afbf0e9e6c5afdd47f55cc073a80715573234aa93f6ce783ad2da6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:bionic` - linux; amd64

```console
$ docker pull swift@sha256:e984495bb2644766a32a0cee9637f59ddb7b5ce789c4b5ecd7e9b6b237ec13f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **723.7 MB (723714489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b345e79799f9aa81b9fdaf4a24f6e52e2e5cef3f9d646db3e2d0824c65b85586`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 21:22:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 31 Jan 2023 21:22:50 GMT
LABEL Description=Docker Container for the Swift programming language
# Tue, 31 Jan 2023 21:25:20 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4-openssl-dev     libxml2-dev     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython3.6     tzdata     git     unzip     pkg-config     && rm -r /var/lib/apt/lists/*
# Tue, 31 Jan 2023 21:25:21 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 31 Jan 2023 21:25:22 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Tue, 31 Jan 2023 21:25:22 GMT
ARG SWIFT_BRANCH=swift-5.7.3-release
# Tue, 31 Jan 2023 21:25:22 GMT
ARG SWIFT_VERSION=swift-5.7.3-RELEASE
# Tue, 31 Jan 2023 21:25:22 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 31 Jan 2023 21:25:22 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.7.3-release SWIFT_VERSION=swift-5.7.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 31 Jan 2023 21:26:07 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Tue, 31 Jan 2023 21:26:13 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922daafa9d1d69c9adb280319dd75f9535a9b5e090a1b105c16c50ef7b214c0c`  
		Last Modified: Tue, 31 Jan 2023 22:00:47 GMT  
		Size: 151.9 MB (151869311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a6b8bfa3e3c99e9f81529c51670fc6324b59174720eb446589f06aeed20aed`  
		Last Modified: Tue, 31 Jan 2023 22:01:39 GMT  
		Size: 545.1 MB (545133356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790eff0bd6cb04065e17e8cc40705f8046b362580844d8935938da4a3eec19e5`  
		Last Modified: Tue, 31 Jan 2023 22:00:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
