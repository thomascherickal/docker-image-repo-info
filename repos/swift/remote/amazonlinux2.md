## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:2d1244622f9ad27bbc1524e5219bef7739ed88aa03578d9456d9a3c7e5f38808
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:e29b57482bc815ef6e11298320fb4e0e3c836765a6b2e8eeada1319faea8a133
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **902.3 MB (902278713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddcf4c29c24f00fa5c13d3a6c4761390082e5fa68c6a0b7bedf6debb1ab7d56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Mar 2023 01:20:24 GMT
COPY dir:1fe253a28ffa7545ac05b2d6b2410c0b48083e8195b6557287b6a94e845122d3 in / 
# Fri, 10 Mar 2023 01:20:24 GMT
CMD ["/bin/bash"]
# Fri, 10 Mar 2023 01:46:40 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 10 Mar 2023 01:46:40 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 10 Mar 2023 01:47:12 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Fri, 10 Mar 2023 01:47:14 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 10 Mar 2023 01:47:14 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 10 Mar 2023 01:47:14 GMT
ARG SWIFT_BRANCH=swift-5.7.3-release
# Fri, 10 Mar 2023 01:47:14 GMT
ARG SWIFT_VERSION=swift-5.7.3-RELEASE
# Fri, 10 Mar 2023 01:47:14 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 10 Mar 2023 01:47:15 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.7.3-release SWIFT_VERSION=swift-5.7.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 10 Mar 2023 01:47:57 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 10 Mar 2023 01:48:03 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:07e4d356f367b468402d36db62e60b734522576ce93a8e7246f1b36899c58f5e`  
		Last Modified: Thu, 09 Mar 2023 17:52:43 GMT  
		Size: 62.5 MB (62477005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4d8b60b8505014b157e7616119a75d9cadb7d76c1ec4541adcde2f21acafbc`  
		Last Modified: Fri, 10 Mar 2023 02:05:29 GMT  
		Size: 295.6 MB (295642913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d589c43002e3367360053365e4ec3f4ad2580e48d93b141e40f573801e5bee46`  
		Last Modified: Fri, 10 Mar 2023 02:06:07 GMT  
		Size: 544.2 MB (544158568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d32e502720c2ac8c39f6d8160a7018df3ead57c2003a1ee53af7be79eca611`  
		Last Modified: Fri, 10 Mar 2023 02:04:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:amazonlinux2` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:0bfdff63dfd931644856d73a3eeb5ef466c75d919ee00299d934416bb8e0e97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **844.0 MB (843985548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc259b6a6b11b4ed4fa7739df8064b08f9aa3d2c874cf6e0cd286224ff09ae2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Mar 2023 01:39:35 GMT
COPY dir:1997e4057e1f8b7df06806432d2b2c303c1f6ef5b18e8273d4393b867415d8b2 in / 
# Fri, 10 Mar 2023 01:39:36 GMT
CMD ["/bin/bash"]
# Fri, 10 Mar 2023 01:55:59 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 10 Mar 2023 01:55:59 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 10 Mar 2023 01:56:23 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Fri, 10 Mar 2023 01:56:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 10 Mar 2023 01:56:27 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 10 Mar 2023 01:56:27 GMT
ARG SWIFT_BRANCH=swift-5.7.3-release
# Fri, 10 Mar 2023 01:56:27 GMT
ARG SWIFT_VERSION=swift-5.7.3-RELEASE
# Fri, 10 Mar 2023 01:56:27 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 10 Mar 2023 01:56:27 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.7.3-release SWIFT_VERSION=swift-5.7.3-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 10 Mar 2023 01:57:03 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 10 Mar 2023 01:57:14 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:042c9cfa8a36c0ffe86667a7dd7d488f78cbe295aa845213c01fdf8784165a92`  
		Last Modified: Fri, 10 Mar 2023 01:40:11 GMT  
		Size: 64.1 MB (64125204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6a86983e80130d0a3430e6016a8dcdee106edc06f18fdcaa0fdf4c8900469c`  
		Last Modified: Fri, 10 Mar 2023 02:00:36 GMT  
		Size: 255.5 MB (255498501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3815885215a4485e6c064895868f3aa27e8590f1f1eea13d364c5a8a42c2c8`  
		Last Modified: Fri, 10 Mar 2023 02:01:07 GMT  
		Size: 524.4 MB (524361615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8157cc3132d685d168cf163bd3485453412a7a505e956202565bfbd64ca859de`  
		Last Modified: Fri, 10 Mar 2023 02:00:16 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
