## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:f2a37e930ddc0ab2ae2c52ff0d4e017590133f8eb60b747a7b45631d89a6fd53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:3be93e2b94df6ce6a17c2a12e4c45d7196708a7874d61e4949d8426d6541e2d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **736.4 MB (736373518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a43e3333e1dcdf8fad6f4c5f8880445736e0482dbd4e5faaf37f7830653a2f`
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
# Sat, 30 Jan 2021 02:05:36 GMT
ARG SWIFT_BRANCH=swift-5.3.3-release
# Sat, 30 Jan 2021 02:05:41 GMT
ARG SWIFT_VERSION=swift-5.3.3-RELEASE
# Sat, 30 Jan 2021 02:05:43 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Sat, 30 Jan 2021 02:05:43 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.3.3-release SWIFT_VERSION=swift-5.3.3-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Sat, 30 Jan 2021 02:07:06 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Sat, 30 Jan 2021 02:07:10 GMT
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
	-	`sha256:fca9bc2d7e7fc4fae347737f65943b6781ca1efaec2821afc14aad88d89e2bb6`  
		Last Modified: Sat, 30 Jan 2021 02:23:16 GMT  
		Size: 424.7 MB (424737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
