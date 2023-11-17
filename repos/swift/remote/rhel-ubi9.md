## `swift:rhel-ubi9`

```console
$ docker pull swift@sha256:55993878f31556fe8ba269a3e9c8bc143b91a824d36583912c8c716b9ab1444e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:rhel-ubi9` - linux; amd64

```console
$ docker pull swift@sha256:c9ed098fffb2dc7644d8d87131f6362159d1999829d43b00247f1f6c4dc3fb4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **807.7 MB (807673554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77d062106a6e7bfbe7bff096c1c84bfb00828b85469dc460dcc2d259e9e47dd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Nov 2023 16:57:21 GMT
ADD file:51365bf81ffef571b9cae6537437d1cb9578bf45d8b6a353848d4bbc24583ace in / 
# Thu, 09 Nov 2023 16:57:22 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 09 Nov 2023 16:57:22 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Thu, 09 Nov 2023 16:57:23 GMT
ADD multi:af962ebf871d89c5885926949add253d557f4af2063b876a12e675ae0ac48a6d in /etc/yum.repos.d/ 
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.3"
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL io.openshift.expose-services=""
# Thu, 09 Nov 2023 16:57:23 GMT
LABEL io.openshift.tags="base rhel9"
# Thu, 09 Nov 2023 16:57:23 GMT
ENV container oci
# Thu, 09 Nov 2023 16:57:23 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Nov 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Thu, 09 Nov 2023 16:57:23 GMT
RUN rm -rf /var/log/*
# Thu, 09 Nov 2023 16:57:24 GMT
RUN mkdir -p /var/log/rhsm
# Thu, 09 Nov 2023 16:57:24 GMT
ADD file:b21f5a973eb1a7e7cede8eb88bab4f034175bf01de661263540b4722655ec4b1 in /root/buildinfo/content_manifests/ubi9-container-9.3-1361.1699548029.json 
# Thu, 09 Nov 2023 16:57:25 GMT
ADD file:81c5ce84fbc74763cd36dea9ef0064ee0c92125a77a579cfbb4a026beeb7be4f in /root/buildinfo/Dockerfile-ubi9-9.3-1361.1699548029 
# Thu, 09 Nov 2023 16:57:25 GMT
LABEL "release"="1361.1699548029" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-09T16:40:44" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="eb726081eeafc660c182aae53074ec6631cb473e" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.3-1361.1699548029"
# Thu, 09 Nov 2023 16:57:26 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2540020-1b8c0.repo' '/etc/yum.repos.d/gitweb-15c2e.repo'
# Thu, 09 Nov 2023 16:57:27 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 09 Nov 2023 16:57:29 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 17 Nov 2023 04:17:31 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 17 Nov 2023 04:17:32 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 17 Nov 2023 04:17:53 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Fri, 17 Nov 2023 04:17:54 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 17 Nov 2023 04:17:54 GMT
ARG SWIFT_PLATFORM=ubi9
# Fri, 17 Nov 2023 04:17:54 GMT
ARG SWIFT_BRANCH=swift-5.9.1-release
# Fri, 17 Nov 2023 04:17:54 GMT
ARG SWIFT_VERSION=swift-5.9.1-RELEASE
# Fri, 17 Nov 2023 04:17:54 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 17 Nov 2023 04:17:55 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.9.1-release SWIFT_VERSION=swift-5.9.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 17 Nov 2023 04:18:41 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 17 Nov 2023 04:18:47 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:b824f4b30c465e487e640bdc22e46bafd6983e4e0eabf30085cacf945c261160`  
		Last Modified: Wed, 15 Nov 2023 11:22:54 GMT  
		Size: 78.8 MB (78771519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9147eac6cae0e29431453d2a3a2886e28d88a1a9c6a377ff7e6caa3e989c1dd8`  
		Last Modified: Fri, 17 Nov 2023 04:24:21 GMT  
		Size: 121.8 MB (121778129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c00a38331bb8aacf017dfcb70e3bf66959b073ba12dc25ac16163f8dfcf5fe`  
		Last Modified: Fri, 17 Nov 2023 04:25:27 GMT  
		Size: 607.1 MB (607123705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a2379332fa540892b5d65b28fdb6ad1af0f52d639b4c94c8a50b2a1d64ac2f`  
		Last Modified: Fri, 17 Nov 2023 04:24:06 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:rhel-ubi9` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:c2607ff918e0eb34baf960db2fc73c6cba913a9a60c5753ab040f46816a905d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **794.0 MB (793993138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca7dc688ae5931b72d5f6493809b180164f4697c704371bf625942f796389e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 09 Nov 2023 16:57:17 GMT
ADD file:205960a3d0706f085c18728490f06b5e7fd7a132ab6b07a95a4ed18f00e126f4 in / 
# Thu, 09 Nov 2023 16:57:18 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 09 Nov 2023 16:57:18 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Thu, 09 Nov 2023 16:57:18 GMT
ADD multi:af962ebf871d89c5885926949add253d557f4af2063b876a12e675ae0ac48a6d in /etc/yum.repos.d/ 
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.3"
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL io.openshift.expose-services=""
# Thu, 09 Nov 2023 16:57:18 GMT
LABEL io.openshift.tags="base rhel9"
# Thu, 09 Nov 2023 16:57:18 GMT
ENV container oci
# Thu, 09 Nov 2023 16:57:18 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Nov 2023 16:57:18 GMT
CMD ["/bin/bash"]
# Thu, 09 Nov 2023 16:57:19 GMT
RUN rm -rf /var/log/*
# Thu, 09 Nov 2023 16:57:20 GMT
RUN mkdir -p /var/log/rhsm
# Thu, 09 Nov 2023 16:57:20 GMT
ADD file:0b626ed84dc2ce267bf6b274208582760edaf2c022f3194ac8260153cafce9d1 in /root/buildinfo/content_manifests/ubi9-container-9.3-1361.1699548029.json 
# Thu, 09 Nov 2023 16:57:21 GMT
ADD file:a85c30847dff015a401ef205805a5a71cc706ae037b798d7b69c0465edec50a7 in /root/buildinfo/Dockerfile-ubi9-9.3-1361.1699548029 
# Thu, 09 Nov 2023 16:57:21 GMT
LABEL "release"="1361.1699548029" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-09T16:40:44" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="eb726081eeafc660c182aae53074ec6631cb473e" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.3-1361.1699548029"
# Thu, 09 Nov 2023 16:57:22 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2540020-1b8c0.repo' '/etc/yum.repos.d/gitweb-15c2e.repo'
# Thu, 09 Nov 2023 16:57:23 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 09 Nov 2023 16:57:25 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 17 Nov 2023 03:33:06 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Fri, 17 Nov 2023 03:33:06 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 17 Nov 2023 03:33:24 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Fri, 17 Nov 2023 03:33:26 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 17 Nov 2023 03:33:26 GMT
ARG SWIFT_PLATFORM=ubi9
# Fri, 17 Nov 2023 03:33:26 GMT
ARG SWIFT_BRANCH=swift-5.9.1-release
# Fri, 17 Nov 2023 03:33:26 GMT
ARG SWIFT_VERSION=swift-5.9.1-RELEASE
# Fri, 17 Nov 2023 03:33:26 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Fri, 17 Nov 2023 03:33:26 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.9.1-release SWIFT_VERSION=swift-5.9.1-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Fri, 17 Nov 2023 03:34:11 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Fri, 17 Nov 2023 03:34:23 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:19dd821b7a83bf1ad388914394494ea983308667df914c57a315c52e312eb2c4`  
		Last Modified: Wed, 15 Nov 2023 11:22:52 GMT  
		Size: 76.5 MB (76512185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fc2b349bdc2939f2aecce639b6653edd36f9f850fdccef537fce3ef5d9db32`  
		Last Modified: Fri, 17 Nov 2023 03:38:04 GMT  
		Size: 115.8 MB (115777908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88148505798541ea5c506304e406f4be51fb6b83b9c3b11149acacd8df0209ef`  
		Last Modified: Fri, 17 Nov 2023 03:38:54 GMT  
		Size: 601.7 MB (601702845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f961a494086fe6ed78a9034e03cbfe314c899ce82e3c588e34d2c2e9d461298`  
		Last Modified: Fri, 17 Nov 2023 03:37:53 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
