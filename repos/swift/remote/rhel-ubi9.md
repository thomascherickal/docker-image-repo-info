## `swift:rhel-ubi9`

```console
$ docker pull swift@sha256:8322745f3a481426e8cdb84b6d8d654ff957593d82e29be2135349aee5a7da88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:rhel-ubi9` - linux; amd64

```console
$ docker pull swift@sha256:0cf2021191d7672dc3fdd63404243668744ee3106513aae9dd078b7903e4d542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **755.0 MB (754971933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49459f24b97c00b46413c7f3ff3653e78d9b3e5bcd31f101e089fda500ef81cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 04 Apr 2023 13:11:29 GMT
ADD file:8773f383286325a8a39fe04548f58b015caca22d611b996698b5458f50f91c88 in / 
# Tue, 04 Apr 2023 13:11:30 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Tue, 04 Apr 2023 13:11:30 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Tue, 04 Apr 2023 13:11:30 GMT
ADD multi:b69fbca1cffcb1fb28acb34486e2a3bc449bb345809fd618d7d6606c2a083b31 in /etc/yum.repos.d/ 
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL maintainer="Red Hat, Inc."
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.1.0"
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL io.openshift.expose-services=""
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL io.openshift.tags="base rhel9"
# Tue, 04 Apr 2023 13:11:30 GMT
ENV container oci
# Tue, 04 Apr 2023 13:11:30 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 13:11:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Apr 2023 13:11:31 GMT
RUN rm -rf /var/log/*
# Tue, 04 Apr 2023 13:11:31 GMT
RUN mkdir -p /var/log/rhsm
# Tue, 04 Apr 2023 13:11:31 GMT
LABEL release=1817
# Tue, 04 Apr 2023 13:11:31 GMT
ADD file:b651e93bb40065a25f26c10e2357508f9447e94b79dcb190dfa86ba427333b56 in /root/buildinfo/content_manifests/ubi9-container-9.1.0-1817.json 
# Tue, 04 Apr 2023 13:11:32 GMT
ADD file:bcae467fc5315f9d3aac6609cb0e25312849de600526a5e7a993c594dd872c72 in /root/buildinfo/Dockerfile-ubi9-9.1.0-1817 
# Tue, 04 Apr 2023 13:11:32 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-04-04T12:59:33" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="cf87ad00feaef3d9d7a442dad55ab6a14f6a3f81" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.1.0-1817"
# Tue, 04 Apr 2023 13:11:32 GMT
RUN rm -f '/etc/yum.repos.d/repo-6b42c.repo' '/etc/yum.repos.d/repo-8e12e.repo'
# Tue, 04 Apr 2023 13:11:33 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Tue, 04 Apr 2023 13:11:34 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 13 Apr 2023 00:06:38 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 13 Apr 2023 00:06:38 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 13 Apr 2023 00:06:55 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Thu, 13 Apr 2023 00:06:56 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 13 Apr 2023 00:06:56 GMT
ARG SWIFT_PLATFORM=ubi9
# Thu, 13 Apr 2023 00:06:56 GMT
ARG SWIFT_BRANCH=swift-5.8-release
# Thu, 13 Apr 2023 00:06:56 GMT
ARG SWIFT_VERSION=swift-5.8-RELEASE
# Thu, 13 Apr 2023 00:06:56 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 13 Apr 2023 00:06:56 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.8-release SWIFT_VERSION=swift-5.8-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 13 Apr 2023 00:07:29 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Thu, 13 Apr 2023 00:07:34 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:72d37ae8760a66c6d3507cc766ab29e2e49082a565e2a531e4b0bea3c4385392`  
		Last Modified: Wed, 12 Apr 2023 00:07:57 GMT  
		Size: 79.1 MB (79141222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790cbb6f8c211a7e68c1eb3c83a002b7d10f30f951b0526f04539f9988512cb`  
		Last Modified: Thu, 13 Apr 2023 00:13:55 GMT  
		Size: 119.0 MB (118974769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15668479dc9ba6955b68d678974c6de32f2fd3aec4402364a4c045125b62c7b`  
		Last Modified: Thu, 13 Apr 2023 00:14:54 GMT  
		Size: 556.9 MB (556855716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d923db1e289efc364825d076fd505d2b361b04bf228345e8ec8a6c9f40036f`  
		Last Modified: Thu, 13 Apr 2023 00:13:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:rhel-ubi9` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:f8fcbfed8ddba0a611a99a62c7a8bbb8b0cad13bc096c71703189a8502b72461
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **734.6 MB (734592089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6696c81a45a1c0561f5d3cd4daed62c331e034e8c0a171f7e0ceb3a356b95c64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 04 Apr 2023 13:11:29 GMT
ADD file:a8a51120466817aec6fd188298e195876efc062bc0a32b6ba950e7197003b7e5 in / 
# Tue, 04 Apr 2023 13:11:30 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Tue, 04 Apr 2023 13:11:30 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Tue, 04 Apr 2023 13:11:30 GMT
ADD multi:b69fbca1cffcb1fb28acb34486e2a3bc449bb345809fd618d7d6606c2a083b31 in /etc/yum.repos.d/ 
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL maintainer="Red Hat, Inc."
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.1.0"
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL io.openshift.expose-services=""
# Tue, 04 Apr 2023 13:11:30 GMT
LABEL io.openshift.tags="base rhel9"
# Tue, 04 Apr 2023 13:11:30 GMT
ENV container oci
# Tue, 04 Apr 2023 13:11:30 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 13:11:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Apr 2023 13:11:31 GMT
RUN rm -rf /var/log/*
# Tue, 04 Apr 2023 13:11:32 GMT
RUN mkdir -p /var/log/rhsm
# Tue, 04 Apr 2023 13:11:32 GMT
LABEL release=1817
# Tue, 04 Apr 2023 13:11:32 GMT
ADD file:38cefb1bfc1025b78407484c723e4f0ae867a2123422a2f7ecb3960b8b66b647 in /root/buildinfo/content_manifests/ubi9-container-9.1.0-1817.json 
# Tue, 04 Apr 2023 13:11:33 GMT
ADD file:4d60f7fbcaa0ce134c8e3b981bf49823d87d0c4183f15e2764860674d1557672 in /root/buildinfo/Dockerfile-ubi9-9.1.0-1817 
# Tue, 04 Apr 2023 13:11:33 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-04-04T12:59:33" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="cf87ad00feaef3d9d7a442dad55ab6a14f6a3f81" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.1.0-1817"
# Tue, 04 Apr 2023 13:11:34 GMT
RUN rm -f '/etc/yum.repos.d/repo-6b42c.repo' '/etc/yum.repos.d/repo-8e12e.repo'
# Tue, 04 Apr 2023 13:11:35 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Tue, 04 Apr 2023 13:11:37 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 12 Apr 2023 20:57:08 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Wed, 12 Apr 2023 20:57:08 GMT
LABEL description=Docker Container for the Swift programming language
# Wed, 12 Apr 2023 20:57:21 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Wed, 12 Apr 2023 20:57:22 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Wed, 12 Apr 2023 20:57:22 GMT
ARG SWIFT_PLATFORM=ubi9
# Wed, 12 Apr 2023 20:57:22 GMT
ARG SWIFT_BRANCH=swift-5.8-release
# Wed, 12 Apr 2023 20:57:23 GMT
ARG SWIFT_VERSION=swift-5.8-RELEASE
# Wed, 12 Apr 2023 20:57:23 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 12 Apr 2023 20:57:23 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.8-release SWIFT_VERSION=swift-5.8-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 12 Apr 2023 20:57:55 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 12 Apr 2023 20:58:06 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:0a38252331b4f7261cd38c165f0ea85731851d23b31cd364fb04327b27347061`  
		Last Modified: Wed, 12 Apr 2023 00:08:18 GMT  
		Size: 76.8 MB (76817165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a7cf85ba62c2f9d167cee5d336f70f20dbadec73dad2457496565456ed74`  
		Last Modified: Wed, 12 Apr 2023 20:59:36 GMT  
		Size: 112.9 MB (112941509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fe6403b5cbc1f76875780fab867fd2d35b97fa37950bda34f89e3a601f9e91`  
		Last Modified: Wed, 12 Apr 2023 21:00:24 GMT  
		Size: 544.8 MB (544833186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49c80d51a5d77b9aeb628b9c972ea9cf18e5748ee3d30b1ad27c11a9d0ca5d7`  
		Last Modified: Wed, 12 Apr 2023 20:59:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
