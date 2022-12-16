## `swift:amazonlinux2`

```console
$ docker pull swift@sha256:4ac1263265156f50514e8d8e5162d042b8e7d914511b6be02fc1603afbac6745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:amazonlinux2` - linux; amd64

```console
$ docker pull swift@sha256:5f72a496ee2dc8c4619dacb05143ff68c20211e4baee94ea502df489d8e696d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **897.9 MB (897905263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230fbc5895ea45bc7093272db972e6e88520991288d89a5821c2d1fba1b14fd1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Dec 2022 01:19:49 GMT
ADD file:a69ca7a5499bcd9d6e4317fdbd7256e93be44364bb746f5da10b4268c090bda0 in / 
# Fri, 16 Dec 2022 01:19:50 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 01:40:03 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 16 Dec 2022 01:40:03 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 16 Dec 2022 01:40:39 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Fri, 16 Dec 2022 01:40:41 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 16 Dec 2022 01:40:41 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 16 Dec 2022 18:34:13 GMT
ARG SWIFT_BRANCH=swift-5.7.2-release
# Fri, 16 Dec 2022 18:34:13 GMT
ARG SWIFT_VERSION=swift-5.7.2-RELEASE
# Fri, 16 Dec 2022 18:34:13 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 18:34:13 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.7.2-release SWIFT_VERSION=swift-5.7.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 18:34:58 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 16 Dec 2022 18:35:04 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:5b4a36b5b78f93a5f470cf722b313bb32cddb0f8e0fa0db348059b5c0881b04f`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 62.3 MB (62328625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419334be1847b87fb236ce143faeb128d763e0ff44fec4799c16624c11034f50`  
		Last Modified: Fri, 16 Dec 2022 02:01:56 GMT  
		Size: 291.4 MB (291409959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7a71cf37b731ee7d1198b308137c07df2c95fe0ac1afb1616776564cfcf248`  
		Last Modified: Fri, 16 Dec 2022 18:54:37 GMT  
		Size: 544.2 MB (544166451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efd13fdda8a55ee585ec9810ffa00ad7a82bab673ca2e33db2c484b6e113c7f`  
		Last Modified: Fri, 16 Dec 2022 18:53:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:amazonlinux2` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:203ddfb46e3eca097d1f17bdf12ce23a4b2eb90de06ba57c55b08ab27e634bee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.8 MB (839804439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564727c6581b1d6b1512220be33a535c5f12c58562729d7dd7436831f10db750`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Dec 2022 00:41:05 GMT
ADD file:26a6bf75c84c408d289e5569f13b1c65206966f875cdfc53ded0670cb85e35bf in / 
# Fri, 16 Dec 2022 00:41:07 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 01:06:40 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 16 Dec 2022 01:06:40 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 16 Dec 2022 01:07:04 GMT
RUN yum -y install   binutils   gcc   git   unzip   glibc-static   gzip   libbsd   libcurl-devel   libedit   libicu   libsqlite   libstdc++-static   libuuid   libxml2-devel   tar   tzdata   zlib-devel
# Fri, 16 Dec 2022 01:07:08 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 16 Dec 2022 01:07:08 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 16 Dec 2022 19:06:56 GMT
ARG SWIFT_BRANCH=swift-5.7.2-release
# Fri, 16 Dec 2022 19:06:56 GMT
ARG SWIFT_VERSION=swift-5.7.2-RELEASE
# Fri, 16 Dec 2022 19:06:56 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 19:06:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.7.2-release SWIFT_VERSION=swift-5.7.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 16 Dec 2022 19:07:39 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 16 Dec 2022 19:07:50 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:6cbfee25f0741b3d3f4d2474d904a200cd8404a01aa17813bf3fc3d4ebb551a4`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 64.0 MB (63964214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eab2bc1bb2e8f071a5e921d5b51f892c959bab31ea1a83b3f8a45c21b796848`  
		Last Modified: Fri, 16 Dec 2022 01:11:39 GMT  
		Size: 251.5 MB (251481694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6803319b65054fd5ba03b0c3d35ea92767f2cd26e078e1d78966a4a26f82bae8`  
		Last Modified: Fri, 16 Dec 2022 19:11:47 GMT  
		Size: 524.4 MB (524358305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9380143ca061e22278f7033de3944acea5a58606347217214dcb0a00e48578b7`  
		Last Modified: Fri, 16 Dec 2022 19:10:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
