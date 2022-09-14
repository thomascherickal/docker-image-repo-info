## `swift:focal-slim`

```console
$ docker pull swift@sha256:11bf0c4881de22fe3ac4f221a0f5199d799d87515886ef0a2672e6397b144a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:focal-slim` - linux; amd64

```console
$ docker pull swift@sha256:bacd948007585c38f3beae98038fd6fa07b38ff979c2e82c982798b765b622e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139992220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da7dbc4798858ae244acbab2a5b7427c7e2086d6b1d98dbd07e32ace093ab9f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:52:26 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 02 Sep 2022 05:52:26 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 02 Sep 2022 05:52:36 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:52:36 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 02 Sep 2022 05:52:36 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Wed, 14 Sep 2022 00:33:06 GMT
ARG SWIFT_BRANCH=swift-5.7-release
# Wed, 14 Sep 2022 00:33:06 GMT
ARG SWIFT_VERSION=swift-5.7-RELEASE
# Wed, 14 Sep 2022 00:33:06 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:33:06 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.7-release SWIFT_VERSION=swift-5.7-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:33:39 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b73d25dc3357120baba929fa673d0c291cda6af151e956567d4dbe80a8f517e`  
		Last Modified: Fri, 02 Sep 2022 06:19:22 GMT  
		Size: 22.2 MB (22226760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6032189a3e0fee76e1bac42153b587fe21747cdc713f5f1e6d96a697a8cc5a99`  
		Last Modified: Wed, 14 Sep 2022 00:51:27 GMT  
		Size: 89.2 MB (89192775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:focal-slim` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:c25f0d9fad1aeecf6716b579414eb9cb90a8a37a849eebcdfdcc6916e2a3e4c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129466067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5ba00c967abf43b907429cb1fbc104f84d9fb245f7a9388885c42740356635`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:57:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 02 Sep 2022 06:57:32 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 02 Sep 2022 06:57:46 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libcurl4     libxml2     tzdata     && rm -r /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:57:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 02 Sep 2022 06:57:48 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Mon, 12 Sep 2022 18:59:14 GMT
ARG SWIFT_BRANCH=swift-5.6.3-release
# Mon, 12 Sep 2022 18:59:14 GMT
ARG SWIFT_VERSION=swift-5.6.3-RELEASE
# Mon, 12 Sep 2022 18:59:15 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Sep 2022 18:59:16 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.6.3-release SWIFT_VERSION=swift-5.6.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Sep 2022 18:59:49 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl gnupg && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl gnupg
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf4074a3a2031e454b553e6f8bd9eef50001e40524cfac0834c6c33b2432b66`  
		Last Modified: Fri, 02 Sep 2022 07:00:34 GMT  
		Size: 22.0 MB (22010437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bca8478a9c073d5c7cc5ef18966dcc570701061188b11e680b84c7ccfd2158`  
		Last Modified: Mon, 12 Sep 2022 19:04:13 GMT  
		Size: 80.3 MB (80263813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
