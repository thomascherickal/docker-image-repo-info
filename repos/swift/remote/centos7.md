## `swift:centos7`

```console
$ docker pull swift@sha256:53134dbdf12067589d4c6983bd93c4f725e1a81d19cb9d22ef4a4279b4275246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:centos7` - linux; amd64

```console
$ docker pull swift@sha256:bb8891426f1527028fb696b05a64c389910a3f604459a981c4ccaba218796bae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.9 MB (577876727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb52ebe2be7d59131a44a14b8d632dece93feb61d486b762fd071049ab6a3860`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 00:49:23 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Sat, 14 Nov 2020 00:49:23 GMT
LABEL description=Docker Container for the Swift programming language
# Sat, 14 Nov 2020 00:50:01 GMT
RUN yum install shadow-utils.x86_64 -y   binutils   gcc   git   glibc-static   libbsd-devel   libedit   libedit-devel   libicu-devel   libstdc++-static   pkg-config   python2   sqlite   zlib-devel
# Sat, 14 Nov 2020 00:50:03 GMT
RUN sed -i -e 's/\*__block/\*__libc_block/g' /usr/include/unistd.h
# Sat, 14 Nov 2020 00:50:03 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Sat, 14 Nov 2020 00:50:03 GMT
ARG SWIFT_PLATFORM=centos7
# Sat, 30 Jan 2021 02:11:52 GMT
ARG SWIFT_BRANCH=swift-5.3.3-release
# Sat, 30 Jan 2021 02:11:52 GMT
ARG SWIFT_VERSION=swift-5.3.3-RELEASE
# Sat, 30 Jan 2021 02:11:52 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Sat, 30 Jan 2021 02:11:52 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos7 SWIFT_BRANCH=swift-5.3.3-release SWIFT_VERSION=swift-5.3.3-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Sat, 30 Jan 2021 02:13:12 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Sat, 30 Jan 2021 02:13:14 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e11ba65f6018a627db410975c668faf65ae6026d9196b753f0731c3d790216e`  
		Last Modified: Sat, 14 Nov 2020 00:57:36 GMT  
		Size: 84.0 MB (83995139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b00d84d6c8da10cb5d583ce36bc8ff7ea0dd5656674dd6dc6bff1c685f3cb5`  
		Last Modified: Sat, 14 Nov 2020 00:57:21 GMT  
		Size: 11.5 KB (11497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57555ef52533ff261d138680559c5997fedae8c09b18217de934c00920547bfc`  
		Last Modified: Sat, 30 Jan 2021 02:26:39 GMT  
		Size: 417.8 MB (417772934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
