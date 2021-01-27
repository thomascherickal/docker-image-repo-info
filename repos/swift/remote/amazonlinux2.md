## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:66f1664e42711223b522d7b2426424cc3801c0b5ff94782a7f9ca13bb764dd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:13c801aad0ffc58deb2be6e94163ac823fb00c736046bd5478a7472ec3653f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **736.3 MB (736254130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94495db06cbde61ba6047356ae7eb7b234cfbd602745d64613732a39bd212c68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:19:43 GMT
ADD file:bcd0b903093ee2c81a54e8bdc50176f4038662ab936aa0d94af08458d508aef6 in / 
# Wed, 27 Jan 2021 22:19:43 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:41:47 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Wed, 27 Jan 2021 22:41:47 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 27 Jan 2021 22:42:16 GMT
RUN yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2   tar   tzdata   zlib-devel
# Wed, 27 Jan 2021 22:42:17 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 27 Jan 2021 22:42:17 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Wed, 27 Jan 2021 22:42:17 GMT
ARG SWIFT_BRANCH=swift-5.3.2-release
# Wed, 27 Jan 2021 22:42:17 GMT
ARG SWIFT_VERSION=swift-5.3.2-RELEASE
# Wed, 27 Jan 2021 22:42:17 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 27 Jan 2021 22:42:17 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.3.2-release SWIFT_VERSION=swift-5.3.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Wed, 27 Jan 2021 22:43:40 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 27 Jan 2021 22:43:42 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:62350c28fdb7b7cbd0e199dd893555ed129ed85da482d882b1eeb574988ea7d6`  
		Last Modified: Wed, 27 Jan 2021 22:21:18 GMT  
		Size: 62.0 MB (61996576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6afe7154d638085698338536a49cea2a58309d94785e75384f46600d427ff8`  
		Last Modified: Wed, 27 Jan 2021 22:52:04 GMT  
		Size: 249.6 MB (249639616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e72283a78447719d9660f4827cfd3b3696c07f56a88de94158adc7193251763`  
		Last Modified: Wed, 27 Jan 2021 22:52:44 GMT  
		Size: 424.6 MB (424617938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
