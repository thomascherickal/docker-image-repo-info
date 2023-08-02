## `swift:rhel-ubi9-slim`

```console
$ docker pull swift@sha256:8bdffff74075d97b216d38a501d02085023636647024657eb92b8228ebb5c74a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:rhel-ubi9-slim` - linux; amd64

```console
$ docker pull swift@sha256:8f2d6b3c2f75d78815ebb15bd964f4fbb7c3b10434cd415b40deef87e2844da8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.2 MB (166176262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1bda52a5e39e05a2806793b9e4b8885f5fc7f502e7061aaf37b16c5628a88a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Jul 2023 14:58:33 GMT
ADD file:40c9f4d78a8d384203610ded7a05dafdbdcf40ae9ca634c63b4b6cd02baf6faf in / 
# Wed, 26 Jul 2023 14:58:33 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 26 Jul 2023 14:58:33 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 26 Jul 2023 14:58:34 GMT
ADD multi:75455514cbe77ce7631a7c71aa7d7e34aff7f5078c6874650e6f91efe6e4c042 in /etc/yum.repos.d/ 
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.2"
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL io.openshift.expose-services=""
# Wed, 26 Jul 2023 14:58:34 GMT
LABEL io.openshift.tags="base rhel9"
# Wed, 26 Jul 2023 14:58:34 GMT
ENV container oci
# Wed, 26 Jul 2023 14:58:34 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 14:58:34 GMT
CMD ["/bin/bash"]
# Wed, 26 Jul 2023 14:58:34 GMT
RUN rm -rf /var/log/*
# Wed, 26 Jul 2023 14:58:35 GMT
RUN mkdir -p /var/log/rhsm
# Wed, 26 Jul 2023 14:58:35 GMT
LABEL release=722
# Wed, 26 Jul 2023 14:58:35 GMT
ADD file:f2acad969853dc6dcc04b456342f7c10e6fa5523796075cea10678ad6c63be0a in /root/buildinfo/content_manifests/ubi9-container-9.2-722.json 
# Wed, 26 Jul 2023 14:58:35 GMT
ADD file:e210e84ce48c52449512909d8b10f94910b5a68dd8b3108bc2b5b7e245fa4832 in /root/buildinfo/Dockerfile-ubi9-9.2-722 
# Wed, 26 Jul 2023 14:58:35 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-07-26T14:47:43" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="6b5892a11894993e819f9a93ee1d7aaa80dc3a17" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.2-722"
# Wed, 26 Jul 2023 14:58:36 GMT
RUN rm -f '/etc/yum.repos.d/repo-ede3e.repo' '/etc/yum.repos.d/repo-0937a.repo'
# Wed, 26 Jul 2023 14:58:37 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 26 Jul 2023 14:58:39 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Tue, 01 Aug 2023 23:34:07 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 01 Aug 2023 23:34:07 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 01 Aug 2023 23:35:17 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 01 Aug 2023 23:35:17 GMT
ARG SWIFT_PLATFORM=ubi9
# Tue, 01 Aug 2023 23:35:18 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Tue, 01 Aug 2023 23:35:18 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Tue, 01 Aug 2023 23:35:18 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 01 Aug 2023 23:35:18 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 01 Aug 2023 23:35:49 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
```

-	Layers:
	-	`sha256:d6427437202d4e0b78a8b9f1c11dce44ee9ec18aeca62950e32310445ae4f545`  
		Last Modified: Tue, 01 Aug 2023 12:05:53 GMT  
		Size: 78.1 MB (78072501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f39e2d43665716292dc60f3be6aa59e97092c1acc1fe992a7672459488a28a`  
		Last Modified: Tue, 01 Aug 2023 23:44:14 GMT  
		Size: 88.1 MB (88103761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:rhel-ubi9-slim` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:d42f27a48a15333c5707cc1d44214764aca689e423474374982fa8e51e246165
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161585497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80dc0d7c2078c821bdbd432b2f0c863cf5c6b1cb814a2cf3119f05c2d4f22be0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Jul 2023 14:58:38 GMT
ADD file:f498f69486c06153ac99c0762bf9d72e8c733e3059ac8d2fef1c309174ad2967 in / 
# Wed, 26 Jul 2023 14:58:40 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 26 Jul 2023 14:58:40 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 26 Jul 2023 14:58:40 GMT
ADD multi:75455514cbe77ce7631a7c71aa7d7e34aff7f5078c6874650e6f91efe6e4c042 in /etc/yum.repos.d/ 
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.2"
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL io.openshift.expose-services=""
# Wed, 26 Jul 2023 14:58:40 GMT
LABEL io.openshift.tags="base rhel9"
# Wed, 26 Jul 2023 14:58:40 GMT
ENV container oci
# Wed, 26 Jul 2023 14:58:40 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 14:58:40 GMT
CMD ["/bin/bash"]
# Wed, 26 Jul 2023 14:58:41 GMT
RUN rm -rf /var/log/*
# Wed, 26 Jul 2023 14:58:43 GMT
RUN mkdir -p /var/log/rhsm
# Wed, 26 Jul 2023 14:58:43 GMT
LABEL release=722
# Wed, 26 Jul 2023 14:58:43 GMT
ADD file:034eadf955ec8ec42cbec88314d6441bea7d4721eac5444800053a8eeee8abe9 in /root/buildinfo/content_manifests/ubi9-container-9.2-722.json 
# Wed, 26 Jul 2023 14:58:43 GMT
ADD file:7ad8a6c099b8b49796620e5d451a102baf3c0bf5eaaca370713271fbaeb49525 in /root/buildinfo/Dockerfile-ubi9-9.2-722 
# Wed, 26 Jul 2023 14:58:43 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-07-26T14:47:43" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="6b5892a11894993e819f9a93ee1d7aaa80dc3a17" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.2-722"
# Wed, 26 Jul 2023 14:58:44 GMT
RUN rm -f '/etc/yum.repos.d/repo-ede3e.repo' '/etc/yum.repos.d/repo-0937a.repo'
# Wed, 26 Jul 2023 14:58:45 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 26 Jul 2023 14:58:47 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Tue, 01 Aug 2023 23:59:19 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 01 Aug 2023 23:59:19 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 02 Aug 2023 00:00:27 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 02 Aug 2023 00:00:27 GMT
ARG SWIFT_PLATFORM=ubi9
# Wed, 02 Aug 2023 00:00:27 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Wed, 02 Aug 2023 00:00:27 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Wed, 02 Aug 2023 00:00:28 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 02 Aug 2023 00:00:28 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 02 Aug 2023 00:00:52 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
```

-	Layers:
	-	`sha256:a06671d5e1b975d0708bdd316b2cc567f8945ff4a42df0a1c5d5f5d8ba36615a`  
		Last Modified: Tue, 01 Aug 2023 12:06:01 GMT  
		Size: 75.8 MB (75804347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcba46f6cbe880e949ae7de27fcc1b8ce51d8b21b242430f4d248213170e180b`  
		Last Modified: Wed, 02 Aug 2023 00:03:10 GMT  
		Size: 85.8 MB (85781150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
