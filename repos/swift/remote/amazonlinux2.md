## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:19a7580eca0ff9b343b489068cc2bc15414bcd4d7b1524a8f0ae251b6b9b7013
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:f39a46f3f969a6fe2da747daa71bf6d7e90c0732173ce5542a2985b65c72f494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **927.1 MB (927097396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7737e332abff7c8bbcffc7c463ed8e141ec0e16e44e394a41e0c7710496ea7ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:22 GMT
COPY dir:591ada5c2fb65633b614a3ff732e6d83dcd91fe9ae925844fe9ba3323311bf74 in / 
# Tue, 29 Aug 2023 18:29:23 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:08:21 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 29 Aug 2023 19:08:21 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 29 Aug 2023 19:08:52 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Tue, 29 Aug 2023 19:08:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 29 Aug 2023 19:08:54 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Tue, 29 Aug 2023 19:08:54 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Tue, 29 Aug 2023 19:08:54 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Tue, 29 Aug 2023 19:08:55 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 29 Aug 2023 19:08:55 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 29 Aug 2023 19:09:35 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Tue, 29 Aug 2023 19:09:40 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:8be3d01330d7e2e197495d440aa60d14ac366aad5e8d105d86e384876aefec18`  
		Last Modified: Fri, 25 Aug 2023 08:53:43 GMT  
		Size: 62.5 MB (62477278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567014908b597b9c9a0b7aef64ddd922bdd1da0166b499e0ed921883aee72ecd`  
		Last Modified: Tue, 29 Aug 2023 19:25:47 GMT  
		Size: 309.6 MB (309644503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b4ac75e38864400958598d8937d41a17f9507c9f0d8a7305aefd47e7f74bab`  
		Last Modified: Tue, 29 Aug 2023 19:26:29 GMT  
		Size: 555.0 MB (554975388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be4b861421ae496719fcd7a660e579fe70e734756de79ce88601b741d534c26`  
		Last Modified: Tue, 29 Aug 2023 19:25:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:amazonlinux2` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:50a381fd45d44cb200503fd69216c9c86394a0a33b3ec580e2aef6a71df8eba8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **932.2 MB (932241988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd25b6a606c92b5466220ca696becdd23afa33032b1651fb757991d4054fc5eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 29 Aug 2023 18:41:03 GMT
COPY dir:6fcca547a5a58ffe09e9507247c1ba371889e20efec9c9e016fb6276715fb958 in / 
# Tue, 29 Aug 2023 18:41:04 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 18:57:02 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 29 Aug 2023 18:57:02 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 29 Aug 2023 18:57:27 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Tue, 29 Aug 2023 18:57:31 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 29 Aug 2023 18:57:31 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Wed, 20 Sep 2023 01:57:10 GMT
ARG SWIFT_BRANCH=swift-5.9-release
# Wed, 20 Sep 2023 01:57:10 GMT
ARG SWIFT_VERSION=swift-5.9-RELEASE
# Wed, 20 Sep 2023 01:57:10 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 01:57:10 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.9-release SWIFT_VERSION=swift-5.9-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 20 Sep 2023 01:57:50 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 20 Sep 2023 01:58:02 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:aa4ff431ef8289088d3cf576f166a7c73e7a5dabe3fae46528dbdd9d7194e9e4`  
		Last Modified: Fri, 25 Aug 2023 18:25:09 GMT  
		Size: 64.1 MB (64129994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef3fab8cc9550255cf708b5f29187698fdd7aa2e8ab0fcc4e1efab4cf7210b9`  
		Last Modified: Tue, 29 Aug 2023 19:02:41 GMT  
		Size: 268.9 MB (268904912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af92faac8164bb7f404bef6c4e8a6be145bccbe605b253fefbc755120e4745e`  
		Last Modified: Wed, 20 Sep 2023 02:05:31 GMT  
		Size: 599.2 MB (599206883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7176b0ffeff563e5a3945cf903859d4248560d70f99da6190dae9839e3a67c`  
		Last Modified: Wed, 20 Sep 2023 02:04:31 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
