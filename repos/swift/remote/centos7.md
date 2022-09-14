## `swift:centos7`

```console
$ docker pull swift@sha256:8cd319a269a1e59bca0c0efa35a90099999adfbe1be260caaa5a17876c86be25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:centos7` - linux; amd64

```console
$ docker pull swift@sha256:3a3cbd9e548e9f75744046ee622f6522608afc3909338f2efbdc12750ce6ea51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **814.8 MB (814837875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01de4faf31c5c8cd91e02fbc1bd4e7aea6c0ba5bd9c34ad4400f7bfbd6d3ada`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 23:56:50 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 28 Oct 2021 23:56:50 GMT
LABEL description=Docker Container for the Swift programming language
# Mon, 12 Sep 2022 18:29:45 GMT
RUN yum install shadow-utils.x86_64 -y   binutils   gcc   git   unzip   glibc-static   libbsd-devel   libcurl-devel   libedit   libedit-devel   libicu-devel   libstdc++-static   libxml2-devel   pkg-config   python3   sqlite   zlib-devel
# Mon, 12 Sep 2022 18:29:47 GMT
RUN sed -i -e 's/\*__block/\*__libc_block/g' /usr/include/unistd.h
# Mon, 12 Sep 2022 18:29:47 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 12 Sep 2022 18:29:47 GMT
ARG SWIFT_PLATFORM=centos7
# Wed, 14 Sep 2022 00:36:31 GMT
ARG SWIFT_BRANCH=swift-5.7-release
# Wed, 14 Sep 2022 00:36:31 GMT
ARG SWIFT_VERSION=swift-5.7-RELEASE
# Wed, 14 Sep 2022 00:36:31 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:36:31 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=centos7 SWIFT_BRANCH=swift-5.7-release SWIFT_VERSION=swift-5.7-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:37:19 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 14 Sep 2022 00:37:26 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cf153ce065ef54d83d11b3352a6545dfd22f9957115fb02b8bc021c67daada`  
		Last Modified: Mon, 12 Sep 2022 18:44:30 GMT  
		Size: 197.0 MB (197029788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f65e7a10ed0a06abeb8a0152eedaf1e823e22aab9e7ed0fa711649a48de7974`  
		Last Modified: Mon, 12 Sep 2022 18:44:03 GMT  
		Size: 11.5 KB (11502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa54912249000d4fb7964ec92dfa3c436bfe3ddea864ee0904c8511ccb90f7d2`  
		Last Modified: Wed, 14 Sep 2022 00:56:34 GMT  
		Size: 541.7 MB (541699200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d1439857e2988767ad46bbf9499c57336be5ad69edf2dc4b48c0ecee3a9806`  
		Last Modified: Wed, 14 Sep 2022 00:55:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
