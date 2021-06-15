## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:17731fbeaae203d309cdd41d1b4f94b43e9f3c5bea5bb245db50798f7e07d0a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:4b3efe64788dd5a1e80ccb80e9f57b1348f38950694122507db4b9660b69043e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.6 MB (839641746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f47664fd6c746ac7d226e249e163820bd5d4190b378e041cef0515b6288710`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 14 Jun 2021 22:21:29 GMT
ADD file:7facd6480673cc20118310fb00de5f2fb1f31f41220c1f01c018c356b050e1da in / 
# Mon, 14 Jun 2021 22:21:30 GMT
CMD ["/bin/bash"]
# Mon, 14 Jun 2021 22:42:38 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Mon, 14 Jun 2021 22:42:38 GMT
LABEL description=Docker Container for the Swift programming language
# Mon, 14 Jun 2021 22:43:08 GMT
RUN yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2   tar   tzdata   zlib-devel
# Mon, 14 Jun 2021 22:43:10 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 14 Jun 2021 22:43:10 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Mon, 14 Jun 2021 22:43:10 GMT
ARG SWIFT_BRANCH=swift-5.4.1-release
# Mon, 14 Jun 2021 22:43:11 GMT
ARG SWIFT_VERSION=swift-5.4.1-RELEASE
# Mon, 14 Jun 2021 22:43:11 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Mon, 14 Jun 2021 22:43:11 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.4.1-release SWIFT_VERSION=swift-5.4.1-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Mon, 14 Jun 2021 22:44:41 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Mon, 14 Jun 2021 22:44:47 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:da5a05f6fddb3b2b567304a69bdcf94cf158162626ff7340ffb02dcca421527d`  
		Last Modified: Mon, 14 Jun 2021 22:22:24 GMT  
		Size: 61.9 MB (61949057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6328151ceff2c6800dee250cf2a1d684c528b519013fcb9eca4ace9d47d9a54`  
		Last Modified: Mon, 14 Jun 2021 22:56:26 GMT  
		Size: 258.1 MB (258145965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff4d22132140feb371bd29bbd376db8c2c26ebe3caea59706a63933b61d63dd`  
		Last Modified: Mon, 14 Jun 2021 22:57:13 GMT  
		Size: 519.5 MB (519546724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
