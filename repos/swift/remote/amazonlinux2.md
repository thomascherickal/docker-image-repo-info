## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:db38458361066179d9b58592e6ae7a1635115190942a30f296096151284082c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:96e40d3ae4a815de2093bbe411ee96a22ffecff523fb13a9a6a8290916671ed3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **877.9 MB (877895838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa117236c9e395537269a1be1b668399594d363b84461983cd42fb242ecb59d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 03:06:36 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 12 Aug 2022 03:06:36 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 12 Aug 2022 03:07:10 GMT
RUN yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Fri, 12 Aug 2022 03:07:12 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 12 Aug 2022 03:07:12 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 12 Aug 2022 03:07:12 GMT
ARG SWIFT_BRANCH=swift-5.6.2-release
# Fri, 12 Aug 2022 03:07:13 GMT
ARG SWIFT_VERSION=swift-5.6.2-RELEASE
# Fri, 12 Aug 2022 03:07:13 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:07:13 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.6.2-release SWIFT_VERSION=swift-5.6.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:07:54 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 12 Aug 2022 03:08:00 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5ad109103bc403a7bf9cb2e747c5321255405e637c2fd3f9269e42bb87cac`  
		Last Modified: Fri, 12 Aug 2022 03:23:38 GMT  
		Size: 290.6 MB (290624893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b3f57167044c048a71d32ccc758921f6941e4cf133f8388ae67fe5095bbce`  
		Last Modified: Fri, 12 Aug 2022 03:24:22 GMT  
		Size: 525.0 MB (524954503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa671fb07224f88ca946748098762547b5c51002e875c9e0a9fc7ba3de3fdd`  
		Last Modified: Fri, 12 Aug 2022 03:23:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:amazonlinux2` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:82479bcdbdb8f5a33b8feb2448eef7dbefc0942a9e95ae4a07962cf2c0dd2755
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **820.2 MB (820157701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962054c28dc5ca1430b136be59a792e917d0a3f6186f8b0043d779f18c60fcde`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:39:26 GMT
ADD file:3ec97c6bec2a8682b0b4088021da97853effeb7dfafb69329cfcb5686c3dee30 in / 
# Fri, 12 Aug 2022 00:39:28 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 03:24:42 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 12 Aug 2022 03:24:43 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 12 Aug 2022 03:25:09 GMT
RUN yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Fri, 12 Aug 2022 03:25:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 12 Aug 2022 03:25:11 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 12 Aug 2022 03:25:12 GMT
ARG SWIFT_BRANCH=swift-5.6.2-release
# Fri, 12 Aug 2022 03:25:13 GMT
ARG SWIFT_VERSION=swift-5.6.2-RELEASE
# Fri, 12 Aug 2022 03:25:14 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:25:15 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.6.2-release SWIFT_VERSION=swift-5.6.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 12 Aug 2022 03:26:02 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 12 Aug 2022 03:26:04 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:9f9c648afd7976bdc42d03595d6a1c1c502c47f18abb3f42a9a20b38e7d6e161`  
		Last Modified: Mon, 01 Aug 2022 22:09:01 GMT  
		Size: 63.9 MB (63927916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c0262217b2fdda819f20bd54465584e5578376d66a0b8b1bfc9af84a35dbb1`  
		Last Modified: Fri, 12 Aug 2022 03:27:53 GMT  
		Size: 251.1 MB (251056406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff723c697d25711222c9aa373a2068450cdde58d282d4c9e39acf4ea2cf04cde`  
		Last Modified: Thu, 16 Jun 2022 17:47:12 GMT  
		Size: 505.2 MB (505173179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e881ab9769bcc2222736da9c1901b4e48a2f48fdbe2378448877a43ded1bdec9`  
		Last Modified: Fri, 12 Aug 2022 03:27:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
