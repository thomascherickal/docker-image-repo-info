## `eclipse-temurin:8u382-b05-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:3dd01db2e5f2867a8b67f204e00c804164548a565b8bcf709e875b3d7aac0e5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:8u382-b05-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:99dbc3245b958f5b6b98a64b5cc2c2d7efda91368b69f7e73e375adf23e589b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107577474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b06fce9f99884add8b255c283494ee9bf54946481f149ff6d1d593657ca1edc`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 09:12:43 GMT
ADD file:941e8e63c7dda0f8bbbf5b9262a1b27948be3557d23e6a486c71b35a2c1bc4c2 in / 
# Tue, 05 Sep 2023 09:12:43 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Tue, 05 Sep 2023 09:12:44 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Tue, 05 Sep 2023 09:12:44 GMT
ADD multi:724ed0e3f3beae9b8bce7fd72262ce34617b5e89ed2a1257879bb55c22d53483 in /etc/yum.repos.d/ 
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL maintainer="Red Hat, Inc."
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL io.openshift.expose-services=""
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL io.openshift.tags="minimal rhel9"
# Tue, 05 Sep 2023 09:12:44 GMT
ENV container oci
# Tue, 05 Sep 2023 09:12:44 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Sep 2023 09:12:44 GMT
CMD ["/bin/bash"]
# Tue, 05 Sep 2023 09:12:44 GMT
RUN rm -rf /var/log/*
# Tue, 05 Sep 2023 09:12:44 GMT
LABEL release=750
# Tue, 05 Sep 2023 09:12:45 GMT
ADD file:dd357e6a9eb4775817d5b3661766c059b0f8be7495521c94f4a1996e79b296af in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-750.json 
# Tue, 05 Sep 2023 09:12:45 GMT
ADD file:a135e818743f081adf270787e41a0c86edf6d9e4a7555d04157dac6afbec26c4 in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-750 
# Tue, 05 Sep 2023 09:12:45 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-09-05T09:00:56" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-750"
# Tue, 05 Sep 2023 09:12:45 GMT
RUN rm -f '/etc/yum.repos.d/repo-f8785.repo' '/etc/yum.repos.d/repo-08a34.repo'
# Tue, 05 Sep 2023 09:12:46 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Tue, 05 Sep 2023 09:12:47 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 13 Sep 2023 00:12:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 13 Sep 2023 00:12:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Sep 2023 00:12:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 13 Sep 2023 00:12:18 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Wed, 13 Sep 2023 00:12:18 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 13 Sep 2023 00:12:44 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 13 Sep 2023 00:12:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 13 Sep 2023 00:12:44 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 13 Sep 2023 00:12:45 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:35e8d0567610305e5133f45eac553d3f57e4f33e2f764a1f16bab4f3bf24ad86`  
		Last Modified: Tue, 12 Sep 2023 17:06:17 GMT  
		Size: 37.9 MB (37869610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4b2d8ae9950ba9ad7cdcc984cea26a412f3c27beebefa591575d2a8cddac7a`  
		Last Modified: Wed, 13 Sep 2023 00:16:03 GMT  
		Size: 27.9 MB (27861943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51308e4ebd6e60e485e8afb0aa29b7890620355120addba35f16a52a01dd1b3b`  
		Last Modified: Wed, 13 Sep 2023 00:16:29 GMT  
		Size: 41.8 MB (41845051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215b557dec22322e8bbeda219c834797d7f1f4796ba4c3799ba183c789649adc`  
		Last Modified: Wed, 13 Sep 2023 00:16:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fce25b9b18dcbcab9b8d1c0c9afdeaf29e19e115ea180169943893d46ded8b`  
		Last Modified: Wed, 13 Sep 2023 00:16:24 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u382-b05-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:32840ba4011a9672903624c27f1ed1884c8b0274b636100ba20e1da460c99b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105265261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffb1ed12be5acae34acdcef412bfc8f2c0a957df747f3bf60d58f4a94ef0697`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 26 Jul 2023 14:58:04 GMT
ADD file:8d7c0f622c108d1e429ca4709a9dda0c55a5dd4cf1e5e2870676045dce7caeba in / 
# Wed, 26 Jul 2023 14:58:05 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 26 Jul 2023 14:58:05 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 26 Jul 2023 14:58:05 GMT
ADD multi:75455514cbe77ce7631a7c71aa7d7e34aff7f5078c6874650e6f91efe6e4c042 in /etc/yum.repos.d/ 
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL io.openshift.expose-services=""
# Wed, 26 Jul 2023 14:58:05 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 26 Jul 2023 14:58:05 GMT
ENV container oci
# Wed, 26 Jul 2023 14:58:05 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 14:58:05 GMT
CMD ["/bin/bash"]
# Wed, 26 Jul 2023 14:58:07 GMT
RUN rm -rf /var/log/*
# Wed, 26 Jul 2023 14:58:07 GMT
LABEL release=717
# Wed, 26 Jul 2023 14:58:07 GMT
ADD file:14e3121d95013deb0e4913aeb325fcf7bbf604080f2fc69e396fcf1a88bc8897 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-717.json 
# Wed, 26 Jul 2023 14:58:07 GMT
ADD file:ba1f369d1b07d713c5215a52333de8398076c4ecb9e2b6628520422b2da2b65a in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-717 
# Wed, 26 Jul 2023 14:58:07 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-07-26T14:47:44" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-717"
# Wed, 26 Jul 2023 14:58:08 GMT
RUN rm -f '/etc/yum.repos.d/repo-ede3e.repo' '/etc/yum.repos.d/repo-0937a.repo'
# Wed, 26 Jul 2023 14:58:09 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 26 Jul 2023 14:58:11 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 02 Aug 2023 00:03:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Aug 2023 00:03:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Aug 2023 00:03:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Aug 2023 00:03:52 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Wed, 02 Aug 2023 00:03:52 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 02 Aug 2023 00:04:12 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 02 Aug 2023 00:04:13 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Mon, 14 Aug 2023 18:09:06 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:06 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:9624f58f605cb9332696a166f1617f4e6d7fb1060bba9b0ea2aac67daac0dc73`  
		Last Modified: Tue, 01 Aug 2023 12:07:13 GMT  
		Size: 36.1 MB (36130176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78179c51ffbc35adfff015fcabffcfccefa9d8913285f7c8e6fecba7de53d28b`  
		Last Modified: Wed, 02 Aug 2023 00:06:38 GMT  
		Size: 28.3 MB (28290560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bd2021d6704788a7fbcc9aa98bd338106e4556ab54905e9f9319f7b50f7f66`  
		Last Modified: Wed, 02 Aug 2023 00:07:02 GMT  
		Size: 40.8 MB (40843654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf00000535aacc190dd46eaf0b0524756492de2c737f0d5f1f794f43854af823`  
		Last Modified: Wed, 02 Aug 2023 00:06:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84252c64d79ff06cbebbded187114f59e4dcbd401627a29046e3af8599c258`  
		Last Modified: Mon, 14 Aug 2023 18:11:51 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u382-b05-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:8e42631d732a8e95861e4f3820a983a2099f9ba3d4d72105bcdf18a90aef4910
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113939181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1411687660c4986cf06a3f6d6d578e432815a38c78a317c18f742b92b17e32cd`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 26 Jul 2023 14:57:48 GMT
ADD file:0c441962aa29a3affc408ed5089865900d38e4b549824783248a665571d42ebf in / 
# Wed, 26 Jul 2023 14:57:50 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 26 Jul 2023 14:57:50 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 26 Jul 2023 14:57:50 GMT
ADD multi:75455514cbe77ce7631a7c71aa7d7e34aff7f5078c6874650e6f91efe6e4c042 in /etc/yum.repos.d/ 
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL io.openshift.expose-services=""
# Wed, 26 Jul 2023 14:57:50 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 26 Jul 2023 14:57:50 GMT
ENV container oci
# Wed, 26 Jul 2023 14:57:50 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 14:57:50 GMT
CMD ["/bin/bash"]
# Wed, 26 Jul 2023 14:57:51 GMT
RUN rm -rf /var/log/*
# Wed, 26 Jul 2023 14:57:51 GMT
LABEL release=717
# Wed, 26 Jul 2023 14:57:51 GMT
ADD file:a666bb3210193c7a955c3cec15b42d917e019faddf36ddc2545c81fc7f9ee928 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-717.json 
# Wed, 26 Jul 2023 14:57:52 GMT
ADD file:688393c03d435532347f62afef64019a0b40f85408be8040970afc31de6816e2 in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-717 
# Wed, 26 Jul 2023 14:57:52 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-07-26T14:47:44" "architecture"="ppc64le" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-717"
# Wed, 26 Jul 2023 14:57:53 GMT
RUN rm -f '/etc/yum.repos.d/repo-ede3e.repo' '/etc/yum.repos.d/repo-0937a.repo'
# Wed, 26 Jul 2023 14:57:54 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 26 Jul 2023 14:57:56 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Tue, 01 Aug 2023 23:16:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 01 Aug 2023 23:16:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 23:16:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 01 Aug 2023 23:18:28 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Tue, 01 Aug 2023 23:18:48 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 01 Aug 2023 23:20:15 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Tue, 01 Aug 2023 23:20:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Mon, 14 Aug 2023 18:09:29 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:30 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:8458a49a58a9ceefce8feddf47e6c6d5ac3416b39eddb7e6a86407b47b94d1cb`  
		Last Modified: Tue, 01 Aug 2023 12:07:20 GMT  
		Size: 42.3 MB (42290376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2713fd75507be3000cb44286c34e36d1b211a49c77956a228a83323a08e1d`  
		Last Modified: Tue, 01 Aug 2023 23:26:03 GMT  
		Size: 30.4 MB (30421820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d813e07c5994f9517cda1471aec52d121f199a9eea23feaa0ff6da66c3831c5a`  
		Last Modified: Tue, 01 Aug 2023 23:26:42 GMT  
		Size: 41.2 MB (41226112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbd83222eab6ba5ed4f2ef79a378e9725e74b22300b18aa5ca8a3d5f15782cf`  
		Last Modified: Tue, 01 Aug 2023 23:26:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027e8e054064668a83e42b751b82beb9d2902cbc9a57ece84921c28b62540f05`  
		Last Modified: Mon, 14 Aug 2023 18:13:35 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
