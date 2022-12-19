## `swift:focal`

```console
$ docker pull swift@sha256:b93d105bdb45588ea4c6b16ae0416adc5b132cef4aceb85007497b5b78445d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:focal` - linux; amd64

```console
$ docker pull swift@sha256:3784427498ed774a1ae3b485d5a8c903f9fbf991703c48a3ce5d3a929bb12dce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **693.3 MB (693308386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4007266674a9fb7a6cbab9533c4b77e43169c97b37b8448680842cd5110267d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:57:16 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 09 Dec 2022 02:57:16 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 09 Dec 2022 02:58:39 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     unzip     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:58:40 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 09 Dec 2022 02:58:40 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Fri, 16 Dec 2022 18:33:15 GMT
ARG SWIFT_BRANCH=swift-5.7.2-release
# Fri, 16 Dec 2022 18:33:15 GMT
ARG SWIFT_VERSION=swift-5.7.2-RELEASE
# Fri, 16 Dec 2022 18:33:15 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 18:33:16 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.7.2-release SWIFT_VERSION=swift-5.7.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 18:33:56 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Fri, 16 Dec 2022 18:34:03 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da0da133ce9ad681102875290150707e2770c190a9637de5a268db728133477`  
		Last Modified: Fri, 09 Dec 2022 03:32:33 GMT  
		Size: 120.2 MB (120236447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbfd60813b097d79c677b245a89e4553caea5d44d3bc2c05a54e4d1318578b5`  
		Last Modified: Fri, 16 Dec 2022 18:53:09 GMT  
		Size: 544.5 MB (544494829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be4f0fe9d2c0905e413990b3b8c9875f596f386d15136fdcce770b8921caf56`  
		Last Modified: Fri, 16 Dec 2022 18:51:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:focal` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:e0f1a5e834e25ced2691ecb83e830826651482e48da6ca5f7d6ae5b0a997475a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **658.9 MB (658901663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc555d55b4c1d7893204ed902e56696e0bf14e496fc1d4a7945521af5adb7496`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:20:05 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 09 Dec 2022 02:20:05 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 09 Dec 2022 02:22:11 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     binutils     git     unzip     gnupg2     libc6-dev     libcurl4-openssl-dev     libedit2     libgcc-9-dev     libpython3.8     libsqlite3-0     libstdc++-9-dev     libxml2-dev     libz3-dev     pkg-config     tzdata     zlib1g-dev     && rm -r /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:22:13 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 09 Dec 2022 02:22:13 GMT
ARG SWIFT_PLATFORM=ubuntu20.04
# Fri, 16 Dec 2022 19:05:04 GMT
ARG SWIFT_BRANCH=swift-5.7.2-release
# Fri, 16 Dec 2022 19:05:04 GMT
ARG SWIFT_VERSION=swift-5.7.2-RELEASE
# Fri, 16 Dec 2022 19:05:04 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 19:05:04 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu20.04 SWIFT_BRANCH=swift-5.7.2-release SWIFT_VERSION=swift-5.7.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Mon, 19 Dec 2022 17:37:08 GMT
RUN set -e;     ARCH_NAME="$(dpkg --print-architecture)";     url=;     case "${ARCH_NAME##*-}" in         'amd64')             OS_ARCH_SUFFIX='';             ;;         'arm64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Mon, 19 Dec 2022 17:37:19 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548584df2a369e7e5827480f9d64ecd7c64f1e4e4b775929949040a44d76d423`  
		Last Modified: Fri, 09 Dec 2022 02:27:50 GMT  
		Size: 117.0 MB (116968196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba45e5a45d14cf2f57575cfaa37489c4d6dba903c7eef6981870bd7df214b08`  
		Last Modified: Mon, 19 Dec 2022 17:39:31 GMT  
		Size: 514.7 MB (514740072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b7a84a3ed23fe702df71a29566b5be22e851314b3be0daa3b4638430e5c4e`  
		Last Modified: Mon, 19 Dec 2022 17:38:37 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
