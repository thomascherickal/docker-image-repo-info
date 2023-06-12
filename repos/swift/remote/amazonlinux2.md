## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:79f4bf0273626b5886c5ac949a54bf1582c54b8e06eccc401f0f206a6c38e1f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:c04a18160fcabae6061fb3391f8e8f2162f2161cf019a69c659d8be9928727d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.9 MB (920915517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a21ef4847f640a39dcf8a43b9642239788be9aa9f0df25a5b66f9a536d606c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:20:12 GMT
COPY dir:fcef1a58ca6f7120ef8bf5af7158a168707c721bb2ebb75f4483ac8ec6174c3f in / 
# Mon, 12 Jun 2023 19:20:13 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:48:29 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Mon, 12 Jun 2023 19:48:29 GMT
LABEL description=Docker Container for the Swift programming language
# Mon, 12 Jun 2023 19:48:59 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Mon, 12 Jun 2023 19:49:02 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 12 Jun 2023 19:49:02 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Mon, 12 Jun 2023 19:49:02 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Mon, 12 Jun 2023 19:49:02 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Mon, 12 Jun 2023 19:49:02 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Jun 2023 19:49:02 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Jun 2023 19:49:44 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Mon, 12 Jun 2023 19:49:49 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:8c8d630364ddfad51ca27951f43586450b97e006740d3139ac1c7fc1fa1a48ab`  
		Last Modified: Wed, 07 Jun 2023 18:46:43 GMT  
		Size: 62.5 MB (62493283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813dd885ad3b65020934e4cac00d01c30bacec01102cce05ec0d9ca0000602e5`  
		Last Modified: Mon, 12 Jun 2023 20:07:12 GMT  
		Size: 303.4 MB (303446634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b288a1ec9231d3ef030b92323da5f8107712985c24d36d8ed9a134a91bcff6a`  
		Last Modified: Mon, 12 Jun 2023 20:07:54 GMT  
		Size: 555.0 MB (554975374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79366445812ebd8646e514c56a38ce40fdae4514453f2959e9a6737e94328664`  
		Last Modified: Mon, 12 Jun 2023 20:06:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:amazonlinux2` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:fc8a839de7de9a0fe39bd6ff10efb6cfa1794e4255e67caabe21e16a9d36b566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.7 MB (862737382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52932e8b664510b3463a800f3c1c27112a30896dfe3d64a1d6fa331247509537`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:41 GMT
COPY dir:51df2295aa01017be94f36c53673ecd4aa152aa99ad3c20338f5409440ff57f7 in / 
# Mon, 12 Jun 2023 19:39:42 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 20:04:39 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Mon, 12 Jun 2023 20:04:39 GMT
LABEL description=Docker Container for the Swift programming language
# Mon, 12 Jun 2023 20:05:01 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Mon, 12 Jun 2023 20:05:06 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 12 Jun 2023 20:05:06 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Mon, 12 Jun 2023 20:05:06 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Mon, 12 Jun 2023 20:05:06 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Mon, 12 Jun 2023 20:05:06 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Jun 2023 20:05:06 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Mon, 12 Jun 2023 20:05:43 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Mon, 12 Jun 2023 20:05:54 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:7943399bb3e529e35dfa651db084f8cbc0868d64a866e4cc4c88d2f0043943a8`  
		Last Modified: Wed, 07 Jun 2023 18:37:02 GMT  
		Size: 64.1 MB (64139660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff359ccd9a1578f8e45506036a810e1f70e52a865a00cdb522a62e217209bf9b`  
		Last Modified: Mon, 12 Jun 2023 20:11:18 GMT  
		Size: 263.1 MB (263119470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e23952a99195826fcf72ec345324d8034ed5ad91287cfd6ffce307f6ba403b`  
		Last Modified: Mon, 12 Jun 2023 20:10:46 GMT  
		Size: 535.5 MB (535478026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03888b0dc0f8db278f38a22b8cd2519ecd418ec91cca129ef0dd1f53b3f928ce`  
		Last Modified: Mon, 12 Jun 2023 20:09:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
