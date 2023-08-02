## `swift:rhel-ubi9`

```console
$ docker pull swift@sha256:b03f2187b5fef9e41dd39aed8221f115ffdb3b7ede756e736ea41ad468b34aea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:rhel-ubi9` - linux; amd64

```console
$ docker pull swift@sha256:a9ac70e84644f626c5170afdbc3400a9149039787e734fd07b9f698775337480
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **756.9 MB (756865598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9284c629ea309af8151ec6c9dd788eb29d775bdf3b56e64223285d4f9278a4f7`
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
# Tue, 01 Aug 2023 23:34:21 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Tue, 01 Aug 2023 23:34:22 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 01 Aug 2023 23:34:22 GMT
ARG SWIFT_PLATFORM=ubi9
# Tue, 01 Aug 2023 23:34:22 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Tue, 01 Aug 2023 23:34:22 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Tue, 01 Aug 2023 23:34:23 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 01 Aug 2023 23:34:23 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Tue, 01 Aug 2023 23:35:05 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Tue, 01 Aug 2023 23:35:11 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:d6427437202d4e0b78a8b9f1c11dce44ee9ec18aeca62950e32310445ae4f545`  
		Last Modified: Tue, 01 Aug 2023 12:05:53 GMT  
		Size: 78.1 MB (78072501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a8bb68846cd158843d02b38d663bd2410e35edec8cf5718b963a39ce786e7f`  
		Last Modified: Tue, 01 Aug 2023 23:42:52 GMT  
		Size: 121.5 MB (121538331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89db6c610394a7b0bc74b9076eed5e41617e8abcf5e41dd7de5bf52a0045596`  
		Last Modified: Tue, 01 Aug 2023 23:43:52 GMT  
		Size: 557.3 MB (557254539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dce94c8bd23a2458a412f6a0d7bf9fb201ce39abadceb4b17f918a47433909`  
		Last Modified: Tue, 01 Aug 2023 23:42:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:rhel-ubi9` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:c1f0721a9adb8e0db339b1593ff28d8a1a5d6e96cd0f425ab2c00e4f2c3c41e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **738.8 MB (738830719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbfe275c1db8c5a34bffcadce348746acc47443a3e1da40ebb89964c094eaaa3`
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
# Tue, 01 Aug 2023 23:59:34 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Tue, 01 Aug 2023 23:59:35 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 01 Aug 2023 23:59:35 GMT
ARG SWIFT_PLATFORM=ubi9
# Tue, 01 Aug 2023 23:59:35 GMT
ARG SWIFT_BRANCH=swift-5.8.1-release
# Tue, 01 Aug 2023 23:59:35 GMT
ARG SWIFT_VERSION=swift-5.8.1-RELEASE
# Tue, 01 Aug 2023 23:59:35 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Tue, 01 Aug 2023 23:59:36 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.8.1-release SWIFT_VERSION=swift-5.8.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 02 Aug 2023 00:00:14 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Wed, 02 Aug 2023 00:00:25 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:a06671d5e1b975d0708bdd316b2cc567f8945ff4a42df0a1c5d5f5d8ba36615a`  
		Last Modified: Tue, 01 Aug 2023 12:06:01 GMT  
		Size: 75.8 MB (75804347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d477b5195bdab700f3d398cb4a17f97eac1dd4f88c834a34599a3be208cf27`  
		Last Modified: Wed, 02 Aug 2023 00:02:06 GMT  
		Size: 115.3 MB (115310536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a4d0d36c2dc3ae000659fd472dae6112aa7bbd275276395223e07b46fed60f`  
		Last Modified: Wed, 02 Aug 2023 00:02:49 GMT  
		Size: 547.7 MB (547715608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0df6d12739a455bd70159e85080b5de17603795d519b530016db697cc4da9`  
		Last Modified: Wed, 02 Aug 2023 00:01:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
