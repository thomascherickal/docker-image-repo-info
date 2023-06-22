## `eclipse-temurin:11-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:ac42bc5f8f9737430ba372b37a985fea2375be44fa87b519c407d893dbd3226d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:a2ccdf6b65057eacf6d34b233d2ee70aead1badb4a4ed8482a0773d88a2f30ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109386853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02a81716c6080d3d791a07f10381e752cda1a4269b91a8e460900a3c4af9d36`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 01:53:36 GMT
ADD file:80304e0bef72b7ea92e51e210b2106f2c76929c20237bda1e2504ed5f08a797b in / 
# Thu, 15 Jun 2023 01:53:37 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 15 Jun 2023 01:53:37 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Thu, 15 Jun 2023 01:53:38 GMT
ADD multi:9849bd0aefa7f9f98ad6e5e3688cb1fbc7313bd1a292ba10ed260c50163f7cee in /etc/yum.repos.d/ 
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL io.openshift.expose-services=""
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL io.openshift.tags="minimal rhel9"
# Thu, 15 Jun 2023 01:53:38 GMT
ENV container oci
# Thu, 15 Jun 2023 01:53:38 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 01:53:38 GMT
CMD ["/bin/bash"]
# Thu, 15 Jun 2023 01:53:39 GMT
RUN rm -rf /var/log/*
# Thu, 15 Jun 2023 01:53:39 GMT
LABEL release=691
# Thu, 15 Jun 2023 01:53:39 GMT
ADD file:f9ce97cb03af747b91e8159962dd1fafb4875a94fd8e03fa1bea1e9a7c1ba028 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-691.json 
# Thu, 15 Jun 2023 01:53:39 GMT
ADD file:2ff83eb5063de7c62bc86b57ae37130f3c49c5f7d6920bc96b44baad3134fcb8 in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-691 
# Thu, 15 Jun 2023 01:53:39 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-06-15T01:42:07" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-691"
# Thu, 15 Jun 2023 01:53:40 GMT
RUN rm -f '/etc/yum.repos.d/repo-dc573.repo' '/etc/yum.repos.d/repo-ef080.repo'
# Thu, 15 Jun 2023 01:53:41 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 15 Jun 2023 01:53:42 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 22 Jun 2023 01:08:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 22 Jun 2023 01:08:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 01:08:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 22 Jun 2023 01:08:25 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Thu, 22 Jun 2023 01:09:00 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 22 Jun 2023 01:09:27 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:09:28 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:62742f27dce5ebff467a57ad6bfa680820f3bc534cc313627f8113246276bf0f`  
		Last Modified: Wed, 21 Jun 2023 18:10:35 GMT  
		Size: 37.8 MB (37833161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89fad3074e960a219b14c1d9389a3f59012f3496f87a126808d6aef4ac84ee`  
		Last Modified: Thu, 22 Jun 2023 01:11:48 GMT  
		Size: 27.9 MB (27864943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e572489249f380f738f252fa77b4dfa43586ebde13d41dcd099317f6b1ee65`  
		Last Modified: Thu, 22 Jun 2023 01:12:48 GMT  
		Size: 43.7 MB (43688589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676945bf2c21767f237dd7e3a38dfe7308417ed374d593a6c61ea20e6df2845a`  
		Last Modified: Thu, 22 Jun 2023 01:12:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:6000f1b5d5df16e59960d26d2147368d90cd86608afaf18da694ac11a938101d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106465849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:246027d3548a2560394b8b49f171c984fd54352eba158cfd99e9296693e87e81`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 01:53:37 GMT
ADD file:2ddf47843f2f56bf055d8a2d5a986816d35279705fd72a482cc996e557eb4d0d in / 
# Thu, 15 Jun 2023 01:53:38 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 15 Jun 2023 01:53:38 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Thu, 15 Jun 2023 01:53:38 GMT
ADD multi:9849bd0aefa7f9f98ad6e5e3688cb1fbc7313bd1a292ba10ed260c50163f7cee in /etc/yum.repos.d/ 
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL io.openshift.expose-services=""
# Thu, 15 Jun 2023 01:53:38 GMT
LABEL io.openshift.tags="minimal rhel9"
# Thu, 15 Jun 2023 01:53:38 GMT
ENV container oci
# Thu, 15 Jun 2023 01:53:38 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 01:53:38 GMT
CMD ["/bin/bash"]
# Thu, 15 Jun 2023 01:53:39 GMT
RUN rm -rf /var/log/*
# Thu, 15 Jun 2023 01:53:39 GMT
LABEL release=691
# Thu, 15 Jun 2023 01:53:39 GMT
ADD file:266cf5a0a08ad49bce286a2a6e6ed92bb75eaeccf0647ce1785fde528a6e4ce7 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-691.json 
# Thu, 15 Jun 2023 01:53:39 GMT
ADD file:fd14cf6ab7b729a931fbee6ca52647a4566540b77950a20a9e14019b02a75ae8 in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-691 
# Thu, 15 Jun 2023 01:53:39 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-06-15T01:42:07" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-691"
# Thu, 15 Jun 2023 01:53:41 GMT
RUN rm -f '/etc/yum.repos.d/repo-dc573.repo' '/etc/yum.repos.d/repo-ef080.repo'
# Thu, 15 Jun 2023 01:53:42 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 15 Jun 2023 01:53:43 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 22 Jun 2023 01:22:21 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 22 Jun 2023 01:22:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 01:22:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 22 Jun 2023 01:22:29 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Thu, 22 Jun 2023 01:22:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 22 Jun 2023 01:23:15 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:23:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:4933b799093955850acfb98487d4801e9a478436ebdbe4db2585569f7dfc7a73`  
		Last Modified: Wed, 21 Jun 2023 18:10:47 GMT  
		Size: 36.1 MB (36137191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221abf6c7eabaab989c2b30a6ba34fbf0d167b44ff1c2c8ad78d55925af18fe9`  
		Last Modified: Thu, 22 Jun 2023 01:25:14 GMT  
		Size: 28.3 MB (28296608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bf05f9147f2a415e3d823bff21c931fad4f3827d6977b5516adba670daaee2`  
		Last Modified: Thu, 22 Jun 2023 01:26:14 GMT  
		Size: 42.0 MB (42031890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a13938ea3cead56a59dad41e82c88a8ee8fc9b338f6ce4faa37142aa66184ea`  
		Last Modified: Thu, 22 Jun 2023 01:26:09 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:70b5c7d966496b1252a0035e65305f55a39de7dde8accd32cd34616ef6805545
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111846525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24118b9eddd2605646f19ed99024d7ca936ffdaf11dbafa2538cf1c8f0d77ec4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 01:54:23 GMT
ADD file:c1d758c5131eb31c12267045c3ab457513fcf413dda42a4641fa6e60cf265fd3 in / 
# Thu, 15 Jun 2023 01:54:24 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 15 Jun 2023 01:54:24 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Thu, 15 Jun 2023 01:54:24 GMT
ADD multi:9849bd0aefa7f9f98ad6e5e3688cb1fbc7313bd1a292ba10ed260c50163f7cee in /etc/yum.repos.d/ 
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL io.openshift.expose-services=""
# Thu, 15 Jun 2023 01:54:24 GMT
LABEL io.openshift.tags="minimal rhel9"
# Thu, 15 Jun 2023 01:54:24 GMT
ENV container oci
# Thu, 15 Jun 2023 01:54:24 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 01:54:24 GMT
CMD ["/bin/bash"]
# Thu, 15 Jun 2023 01:54:26 GMT
RUN rm -rf /var/log/*
# Thu, 15 Jun 2023 01:54:26 GMT
LABEL release=691
# Thu, 15 Jun 2023 01:54:26 GMT
ADD file:0eda173520172f76a0b725b37803c57a32c1391cda8419639363f4c2b7f4ac18 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-691.json 
# Thu, 15 Jun 2023 01:54:26 GMT
ADD file:5a376fbc447f597f91a76df815d29f894dce397f746be88bd73c0c852bd868aa in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-691 
# Thu, 15 Jun 2023 01:54:26 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-06-15T01:42:07" "architecture"="ppc64le" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-691"
# Thu, 15 Jun 2023 01:54:27 GMT
RUN rm -f '/etc/yum.repos.d/repo-dc573.repo' '/etc/yum.repos.d/repo-ef080.repo'
# Thu, 15 Jun 2023 01:54:29 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 15 Jun 2023 01:54:30 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 22 Jun 2023 01:15:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 22 Jun 2023 01:15:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 01:15:24 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 22 Jun 2023 01:15:54 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Thu, 22 Jun 2023 01:16:39 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 22 Jun 2023 01:17:21 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:17:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:e3f3a1bf0aa97991a0413fbe9daa5105fc285b24b4e2ac14458522802ff4e0ec`  
		Last Modified: Wed, 21 Jun 2023 18:11:05 GMT  
		Size: 42.3 MB (42261485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76b5a334e3072ec76c9e2fa0cbaea07673b1437abfa3bdd3c23ed0eca21d193`  
		Last Modified: Thu, 22 Jun 2023 01:19:16 GMT  
		Size: 30.4 MB (30423134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9e05ba3ff0b39d27b8aff8208bcb1a8fec73f2cd96e4654dfd26fed536a5d5`  
		Last Modified: Thu, 22 Jun 2023 01:20:36 GMT  
		Size: 39.2 MB (39161746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7b8e054674876cff315aea07ff7bcba63f46cb266c48e549908a4674f822f1`  
		Last Modified: Thu, 22 Jun 2023 01:20:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:47f7fd2c3ad740268bfaa08e295e754c7c27b9585c4246392a30d48f8c52f7a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101582924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23166f040f8641832d3fa5fbc309c8e89e7ac46f194412bad102ca9ed0b4045c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 01:54:11 GMT
ADD file:1775ae97b5220749eab6d9503babb3e1efe0851edd912ad8074b248d97008cc6 in / 
# Thu, 15 Jun 2023 01:54:12 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Thu, 15 Jun 2023 01:54:12 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Thu, 15 Jun 2023 01:54:13 GMT
ADD multi:9849bd0aefa7f9f98ad6e5e3688cb1fbc7313bd1a292ba10ed260c50163f7cee in /etc/yum.repos.d/ 
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL maintainer="Red Hat, Inc."
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL io.openshift.expose-services=""
# Thu, 15 Jun 2023 01:54:13 GMT
LABEL io.openshift.tags="minimal rhel9"
# Thu, 15 Jun 2023 01:54:13 GMT
ENV container oci
# Thu, 15 Jun 2023 01:54:13 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 01:54:13 GMT
CMD ["/bin/bash"]
# Thu, 15 Jun 2023 01:54:14 GMT
RUN rm -rf /var/log/*
# Thu, 15 Jun 2023 01:54:14 GMT
LABEL release=691
# Thu, 15 Jun 2023 01:54:14 GMT
ADD file:432371a4e24db05d750ad4e0b7532faf0193716bb081c6328fb80f0b333cc51d in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-691.json 
# Thu, 15 Jun 2023 01:54:15 GMT
ADD file:24941b7e43d9d830add98ca27ba9e24220a151f9664be0d6bfdf242d07c75fe8 in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-691 
# Thu, 15 Jun 2023 01:54:15 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-06-15T01:42:07" "architecture"="s390x" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-691"
# Thu, 15 Jun 2023 01:54:16 GMT
RUN rm -f '/etc/yum.repos.d/repo-dc573.repo' '/etc/yum.repos.d/repo-ef080.repo'
# Thu, 15 Jun 2023 01:54:17 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Thu, 15 Jun 2023 01:54:19 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Thu, 22 Jun 2023 10:50:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 22 Jun 2023 10:50:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 10:50:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 22 Jun 2023 10:51:12 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Thu, 22 Jun 2023 10:51:16 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 22 Jun 2023 10:52:09 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 10:52:12 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:39b28ee62fc117719f2eda7966033df48e130840bc47191d514b060095150ad3`  
		Last Modified: Wed, 21 Jun 2023 18:11:16 GMT  
		Size: 36.1 MB (36138929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d634303d8e857e7d44c63bde0fba9c4dc0e91855fd9ba333358865a7529b8c0`  
		Last Modified: Thu, 22 Jun 2023 10:53:58 GMT  
		Size: 27.9 MB (27917054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add7802c541fdc3eb528a22bf5be67eb6a25ab015275dc9cef7f2356a64cace7`  
		Last Modified: Thu, 22 Jun 2023 10:54:21 GMT  
		Size: 37.5 MB (37526779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b0e108e0719cd19e984c568e3d82f036e660f6355664afc695fe274ae8c8b3`  
		Last Modified: Thu, 22 Jun 2023 10:54:16 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
