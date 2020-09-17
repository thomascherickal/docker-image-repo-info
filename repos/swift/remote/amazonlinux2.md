## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:96f41b06a4b60084d433b6dad37a4e9caff7ec651b3f41bf6e2d4d48b60b330f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:f2dadbcb634fd8396ab00d0e8f7dd34cb8c183b5791bc92a207920784272384c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **720.5 MB (720481701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae03106b98b7523da0d0b52bccb929ea0b35943e56b77788380c129d2d80b538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:36:52 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 31 Jul 2020 22:36:52 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 11 Aug 2020 19:31:10 GMT
RUN yum -y install   binutils   gcc   git   glibc-static   gzip   libbsd   libcurl   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2   tar   tzdata   zlib-devel
# Tue, 11 Aug 2020 19:31:11 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 11 Aug 2020 19:31:11 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Thu, 17 Sep 2020 22:30:08 GMT
ARG SWIFT_BRANCH=swift-5.3-release
# Thu, 17 Sep 2020 22:30:12 GMT
ARG SWIFT_VERSION=swift-5.3-RELEASE
# Thu, 17 Sep 2020 22:30:12 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Thu, 17 Sep 2020 22:30:13 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.3-release SWIFT_VERSION=swift-5.3-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Thu, 17 Sep 2020 22:31:27 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Thu, 17 Sep 2020 22:31:30 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1f7f1482d89291419d313abf11456331f6d306986f3df6ad19b0d4fc14311f`  
		Last Modified: Tue, 11 Aug 2020 19:47:59 GMT  
		Size: 239.2 MB (239210608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea12f4464d807180a780cc158428d83c547cdf9387173d2f8c56c7385ec3ec7`  
		Last Modified: Thu, 17 Sep 2020 22:47:49 GMT  
		Size: 419.6 MB (419554553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
