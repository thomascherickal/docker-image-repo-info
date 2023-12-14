## `swift:rhel-ubi9`

```console
$ docker pull swift@sha256:9e2afb40d5b5194eabf36de9ad949857c328596416da8108cb5dc2c5ffa50934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swift:rhel-ubi9` - linux; amd64

```console
$ docker pull swift@sha256:856747c4455e206c1c24d762b1279705f10e2218cbcef1887b7717a67e6960e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **807.8 MB (807756612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:763a7a7646ea412ffab9e021ee738e8e03dbf5da304312ec22027a00329a1eb3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 07 Dec 2023 04:21:35 GMT
ADD file:ea714743adb3d3cbb025bd7b23ae6e83243561af30a43428c24bb5060b98f944 in / 
# Thu, 07 Dec 2023 04:21:36 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 07 Dec 2023 04:21:36 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Thu, 07 Dec 2023 04:21:36 GMT
ADD multi:8257bc82024891d335e91a6d5e44bb825bdb87abe8bc1d2ee3fcfb9e8cbecea1 in /etc/yum.repos.d/ 
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.3"
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL io.openshift.expose-services=""
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL io.openshift.tags="base rhel9"
# Thu, 07 Dec 2023 04:21:36 GMT
ENV container oci
# Thu, 07 Dec 2023 04:21:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 04:21:36 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 04:21:37 GMT
RUN rm -rf /var/log/*
# Thu, 07 Dec 2023 04:21:37 GMT
RUN mkdir -p /var/log/rhsm
# Thu, 07 Dec 2023 04:21:37 GMT
LABEL release=1476
# Thu, 07 Dec 2023 04:21:38 GMT
ADD file:12a008f13c27a43ae1c20cfc8fce9e789788cf5f9e58b05eac097f1da7264532 in /root/buildinfo/content_manifests/ubi9-container-9.3-1476.json 
# Thu, 07 Dec 2023 04:21:38 GMT
ADD file:087fc1f80c6960773f6bbeadefe49f1517b288d51bdd258a006c49932b306573 in /root/buildinfo/Dockerfile-ubi9-9.3-1476 
# Thu, 07 Dec 2023 04:21:38 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-12-07T04:10:37" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="eb726081eeafc660c182aae53074ec6631cb473e" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.3-1476"
# Thu, 07 Dec 2023 04:21:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-84783.repo' '/etc/yum.repos.d/repo-186d3.repo'
# Thu, 07 Dec 2023 04:21:39 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 07 Dec 2023 04:21:41 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 14 Dec 2023 01:57:03 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 14 Dec 2023 01:57:03 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 14 Dec 2023 01:57:38 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Thu, 14 Dec 2023 01:57:39 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 14 Dec 2023 01:57:39 GMT
ARG SWIFT_PLATFORM=ubi9
# Thu, 14 Dec 2023 01:57:40 GMT
ARG SWIFT_BRANCH=swift-5.9.2-release
# Thu, 14 Dec 2023 01:57:40 GMT
ARG SWIFT_VERSION=swift-5.9.2-RELEASE
# Thu, 14 Dec 2023 01:57:40 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 14 Dec 2023 01:57:40 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.9.2-release SWIFT_VERSION=swift-5.9.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 14 Dec 2023 01:58:25 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Thu, 14 Dec 2023 01:58:32 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:af8f1220909b07a1e5f84cdced7681921681484322afb359a03650d1bdee69dd`  
		Last Modified: Wed, 13 Dec 2023 18:07:32 GMT  
		Size: 78.8 MB (78834959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa395c44daa9b31e8c1a71ae97ac4c587591e090b46bebd34111600a43809c`  
		Last Modified: Thu, 14 Dec 2023 02:05:13 GMT  
		Size: 121.8 MB (121775756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05b9c0555f1e3a7edf971087702f08cea4a4c6304167159e02774bffd5dfa18`  
		Last Modified: Thu, 14 Dec 2023 02:06:21 GMT  
		Size: 607.1 MB (607145702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea9194d8a3a389fa1ff73245c5d593ce68fe574af43067dc2850959254458f5`  
		Last Modified: Thu, 14 Dec 2023 02:04:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swift:rhel-ubi9` - linux; arm64 variant v8

```console
$ docker pull swift@sha256:87a0903ffb75e3dc22af63602dbb6d8f30c2cc031b147bb9869bac4dbe03e2b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **794.3 MB (794258577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4bfbf07ad422e67052445efefe6f6bf5372111c0e0aa290900ce85bedd54e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 07 Dec 2023 04:21:32 GMT
ADD file:a3e3249a1aff06c8732f1144a2c74cf27450d3c2d5b5f0259b82b1c02dba495c in / 
# Thu, 07 Dec 2023 04:21:33 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 07 Dec 2023 04:21:34 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Thu, 07 Dec 2023 04:21:34 GMT
ADD multi:8257bc82024891d335e91a6d5e44bb825bdb87abe8bc1d2ee3fcfb9e8cbecea1 in /etc/yum.repos.d/ 
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL com.redhat.component="ubi9-container"       name="ubi9"       version="9.3"
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL summary="Provides the latest release of Red Hat Universal Base Image 9."
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL description="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9"
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL io.openshift.expose-services=""
# Thu, 07 Dec 2023 04:21:34 GMT
LABEL io.openshift.tags="base rhel9"
# Thu, 07 Dec 2023 04:21:34 GMT
ENV container oci
# Thu, 07 Dec 2023 04:21:34 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 04:21:34 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 04:21:35 GMT
RUN rm -rf /var/log/*
# Thu, 07 Dec 2023 04:21:36 GMT
RUN mkdir -p /var/log/rhsm
# Thu, 07 Dec 2023 04:21:36 GMT
LABEL release=1476
# Thu, 07 Dec 2023 04:21:36 GMT
ADD file:b192785828c6f8e6e9f57d8bc2caa38943490fa9742fe3774b30e14ef870bc8b in /root/buildinfo/content_manifests/ubi9-container-9.3-1476.json 
# Thu, 07 Dec 2023 04:21:37 GMT
ADD file:e2d1c622975351096f87e91dfcfefa833f2454e49b5410e3237c53324074f3ff in /root/buildinfo/Dockerfile-ubi9-9.3-1476 
# Thu, 07 Dec 2023 04:21:37 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-12-07T04:10:37" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="eb726081eeafc660c182aae53074ec6631cb473e" "io.k8s.description"="The Universal Base Image is designed and engineered to be the base layer for all of your containerized applications, middleware and utilities. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9/images/9.3-1476"
# Thu, 07 Dec 2023 04:21:38 GMT
RUN rm -f '/etc/yum.repos.d/repo-84783.repo' '/etc/yum.repos.d/repo-186d3.repo'
# Thu, 07 Dec 2023 04:21:40 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 07 Dec 2023 04:21:42 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 14 Dec 2023 01:57:05 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Thu, 14 Dec 2023 01:57:05 GMT
LABEL description=Docker Container for the Swift programming language
# Thu, 14 Dec 2023 01:57:41 GMT
RUN yum -y install   git                 gcc-c++             libcurl-devel       libedit-devel       libuuid-devel       libxml2-devel       ncurses-devel       python3-devel       rsync               sqlite-devel        unzip               zip
# Thu, 14 Dec 2023 01:57:42 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Thu, 14 Dec 2023 01:57:43 GMT
ARG SWIFT_PLATFORM=ubi9
# Thu, 14 Dec 2023 01:57:43 GMT
ARG SWIFT_BRANCH=swift-5.9.2-release
# Thu, 14 Dec 2023 01:57:43 GMT
ARG SWIFT_VERSION=swift-5.9.2-RELEASE
# Thu, 14 Dec 2023 01:57:43 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Thu, 14 Dec 2023 01:57:43 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubi9 SWIFT_BRANCH=swift-5.9.2-release SWIFT_VERSION=swift-5.9.2-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Thu, 14 Dec 2023 01:58:19 GMT
RUN set -e;     ARCH_NAME="$(rpm --eval '%{_arch}')";     url=;     case "${ARCH_NAME##*-}" in         'x86_64')             OS_ARCH_SUFFIX='';             ;;         'aarch64')             OS_ARCH_SUFFIX='-aarch64';             ;;         *) echo >&2 "error: unsupported architecture: '$ARCH_NAME'"; exit 1 ;;     esac;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)$OS_ARCH_SUFFIX"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM$OS_ARCH_SUFFIX.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && echo $SWIFT_BIN_URL     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz
# Thu, 14 Dec 2023 01:58:31 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:12c39db55ed0493a18adb10af3039b3df060854cfd92151180715afd88ddfe24`  
		Last Modified: Wed, 13 Dec 2023 18:07:46 GMT  
		Size: 76.5 MB (76498607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfef1cb22620bcf96c88d0f8920e922f1bf9abda8a7067d4a3ec604ed333aa29`  
		Last Modified: Thu, 14 Dec 2023 02:02:35 GMT  
		Size: 115.8 MB (115777617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6e9f91096ff831389a20e430f453450a68eddeb0860fdf7833f8221baa5d3`  
		Last Modified: Thu, 14 Dec 2023 02:03:22 GMT  
		Size: 602.0 MB (601982155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2635f23cf87d7950ae739d04a7d8f24ce1e33d33c3a77e2fd43f2dd1d72d3b84`  
		Last Modified: Thu, 14 Dec 2023 02:02:22 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
