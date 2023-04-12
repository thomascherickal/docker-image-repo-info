## `eclipse-temurin:20_36-jdk-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:a4fc5f059928ded1389dd773950125458a2bf796648ad331e951b3daf64fea2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:20_36-jdk-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:a37734cfd00f763122952c891ed3903802dee20467960fd8aea4cb6b9a089d41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269580644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0849930939e8347e35aa33c6ae6c299f0cb28202abd3b97e0a3c70738d9b6`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 22 Feb 2023 09:35:54 GMT
ADD file:66552cf0ed33bd315636506183be08809f30be80745578cce6fb86457c9f358d in / 
# Wed, 22 Feb 2023 09:35:54 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 22 Feb 2023 09:35:55 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 22 Feb 2023 09:35:55 GMT
ADD multi:0882c44110b6a64b078cdd328390626e44b18b514d5b9b155c169898325afa84 in /etc/yum.repos.d/ 
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.1.0"
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL io.openshift.expose-services=""
# Wed, 22 Feb 2023 09:35:55 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 22 Feb 2023 09:35:55 GMT
ENV container oci
# Wed, 22 Feb 2023 09:35:55 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Feb 2023 09:35:55 GMT
CMD ["/bin/bash"]
# Wed, 22 Feb 2023 09:35:56 GMT
RUN rm -rf /var/log/*
# Wed, 22 Feb 2023 09:35:56 GMT
LABEL release=1793
# Wed, 22 Feb 2023 09:35:56 GMT
ADD file:462e8c4770a8369bea140f5d93c8443bc2a13ea2445c10cbaf56e865c0b2df68 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.1.0-1793.json 
# Wed, 22 Feb 2023 09:35:56 GMT
ADD file:d860ffc75254e4be550f83682c9b94491c28ba0303d19f67ffdfc2cc60cbb04d in /root/buildinfo/Dockerfile-ubi9-minimal-9.1.0-1793 
# Wed, 22 Feb 2023 09:35:56 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-02-22T09:23:20" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="befaf1f5ec7b874aef2651ee1384d51828504eb9" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.1.0-1793"
# Wed, 22 Feb 2023 09:35:57 GMT
RUN rm -f '/etc/yum.repos.d/repo-5af5d.repo' '/etc/yum.repos.d/repo-93eaf.repo'
# Wed, 22 Feb 2023 09:35:57 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 22 Feb 2023 09:35:59 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 01 Mar 2023 00:13:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 00:13:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 00:13:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Mar 2023 00:13:56 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Mon, 27 Mar 2023 20:24:55 GMT
ENV JAVA_VERSION=jdk-20+36
# Mon, 27 Mar 2023 20:25:02 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='980156d37580bd6fec142e02900497984e94c4b819a0c0eb7ce790bfc7c7d920';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='45dde71faf8cbb78fab3c976894259655c8d3de827347f23e0ebe5710921dded';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb6000faf47fffcda8caf01f60097d582728a6fffb6c1b85c8075c674f0c9281';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Mon, 27 Mar 2023 20:25:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 27 Mar 2023 20:25:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ba958a445f00d91e4019b520c467e36e7f5bc07da02f2a87e9ccefbe4a70ff6d`  
		Last Modified: Tue, 28 Feb 2023 12:08:59 GMT  
		Size: 37.9 MB (37852536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc651e6574a99e69220ab0cc2a07e02c18e914ae9d794427c9b65acafcc62eb8`  
		Last Modified: Wed, 01 Mar 2023 00:18:19 GMT  
		Size: 28.9 MB (28924856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee139e8b172c473be67ee1e37de23d7ca0f54fb7441bb82c20dcea79f57077c`  
		Last Modified: Mon, 27 Mar 2023 20:27:42 GMT  
		Size: 202.8 MB (202803073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d4f8e86a6d8aff2a92ae13db2220a38d70c25e5cadc98744f8da657808a3a`  
		Last Modified: Mon, 27 Mar 2023 20:27:27 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20_36-jdk-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:27430002ecaf3393cc75366b56b2022c2fc01a1c6d2c68c8087f30c77e9b6001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.7 MB (266666219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f0a8599884ed9f694bdb1b6a566ebb9c5e63837915070f5bf570fefff7f91c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Apr 2023 13:07:33 GMT
ADD file:afa1c5c010e4cadc5caa512540bfe7a19a2119f5a23c11699f1fc5ebc3791570 in / 
# Tue, 04 Apr 2023 13:07:34 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Tue, 04 Apr 2023 13:07:34 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Tue, 04 Apr 2023 13:07:34 GMT
ADD multi:b69fbca1cffcb1fb28acb34486e2a3bc449bb345809fd618d7d6606c2a083b31 in /etc/yum.repos.d/ 
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL maintainer="Red Hat, Inc."
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.1.0"
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL io.openshift.expose-services=""
# Tue, 04 Apr 2023 13:07:34 GMT
LABEL io.openshift.tags="minimal rhel9"
# Tue, 04 Apr 2023 13:07:34 GMT
ENV container oci
# Tue, 04 Apr 2023 13:07:34 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 13:07:34 GMT
CMD ["/bin/bash"]
# Tue, 04 Apr 2023 13:07:36 GMT
RUN rm -rf /var/log/*
# Tue, 04 Apr 2023 13:07:36 GMT
LABEL release=1829
# Tue, 04 Apr 2023 13:07:36 GMT
ADD file:eeb46db8ece74b6067d83e79285bc2792da01bf3b91d21f47ba014c45d95d345 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.1.0-1829.json 
# Tue, 04 Apr 2023 13:07:36 GMT
ADD file:fa9a9550d67d7b0c75e5937adbdb8e9c5e69c7db36b0059436a49607b7a5ab77 in /root/buildinfo/Dockerfile-ubi9-minimal-9.1.0-1829 
# Tue, 04 Apr 2023 13:07:36 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-04-04T12:58:00" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="befaf1f5ec7b874aef2651ee1384d51828504eb9" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.1.0-1829"
# Tue, 04 Apr 2023 13:07:37 GMT
RUN rm -f '/etc/yum.repos.d/repo-6b42c.repo' '/etc/yum.repos.d/repo-8e12e.repo'
# Tue, 04 Apr 2023 13:07:38 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Tue, 04 Apr 2023 13:07:40 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 12 Apr 2023 21:01:13 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 21:01:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 21:01:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 12 Apr 2023 21:01:21 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Wed, 12 Apr 2023 21:02:32 GMT
ENV JAVA_VERSION=jdk-20+36
# Wed, 12 Apr 2023 21:02:42 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='980156d37580bd6fec142e02900497984e94c4b819a0c0eb7ce790bfc7c7d920';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='45dde71faf8cbb78fab3c976894259655c8d3de827347f23e0ebe5710921dded';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb6000faf47fffcda8caf01f60097d582728a6fffb6c1b85c8075c674f0c9281';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 12 Apr 2023 21:02:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 12 Apr 2023 21:02:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f5f2c7a71685ec0f59198b120b1eeb1b4156a8e348e3278e9af113dbfd938c63`  
		Last Modified: Wed, 12 Apr 2023 00:12:36 GMT  
		Size: 36.2 MB (36175114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae77f5963c85da26562df7a2bf14b3d03b5142a01dc25b3dae1448566af62f8`  
		Last Modified: Wed, 12 Apr 2023 21:03:41 GMT  
		Size: 29.3 MB (29325370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2f37297abf45749de03e164880f5e61a6e52b9825b6983566713c316ca010a`  
		Last Modified: Wed, 12 Apr 2023 21:05:47 GMT  
		Size: 201.2 MB (201165561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a1f1c9075a5a05829fb67f69bbdfd6b95c127283ae772cad838347a50b6b88`  
		Last Modified: Wed, 12 Apr 2023 21:05:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20_36-jdk-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:e624e5c588b772c8038f03dc7b58d49ce3b9035ab421d299f136bb708e868ca5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.5 MB (274488974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c12b54ecf0afb01d1779b3dd920f7357039030fbb0cd1a938854216e42adbcc`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 22 Feb 2023 09:35:59 GMT
ADD file:8935fa06d65d8716bc53943ac3a6e866ae49cc148df5e8d16a878ee52b6797ef in / 
# Wed, 22 Feb 2023 09:36:00 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 22 Feb 2023 09:36:01 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Wed, 22 Feb 2023 09:36:01 GMT
ADD multi:0882c44110b6a64b078cdd328390626e44b18b514d5b9b155c169898325afa84 in /etc/yum.repos.d/ 
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.1.0"
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL io.openshift.expose-services=""
# Wed, 22 Feb 2023 09:36:01 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 22 Feb 2023 09:36:01 GMT
ENV container oci
# Wed, 22 Feb 2023 09:36:01 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Feb 2023 09:36:01 GMT
CMD ["/bin/bash"]
# Wed, 22 Feb 2023 09:36:03 GMT
RUN rm -rf /var/log/*
# Wed, 22 Feb 2023 09:36:03 GMT
LABEL release=1793
# Wed, 22 Feb 2023 09:36:04 GMT
ADD file:d63a31cf12a5e50647910ea5a5f51f665f02223be7aa3f825874a41f11862464 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.1.0-1793.json 
# Wed, 22 Feb 2023 09:36:04 GMT
ADD file:cf92b2b8113b8a4cb17470ab56427ac77f6240d865c26fb0bede45b333ee9473 in /root/buildinfo/Dockerfile-ubi9-minimal-9.1.0-1793 
# Wed, 22 Feb 2023 09:36:04 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-02-22T09:23:20" "architecture"="ppc64le" "vcs-type"="git" "vcs-ref"="befaf1f5ec7b874aef2651ee1384d51828504eb9" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.1.0-1793"
# Wed, 22 Feb 2023 09:36:06 GMT
RUN rm -f '/etc/yum.repos.d/repo-5af5d.repo' '/etc/yum.repos.d/repo-93eaf.repo'
# Wed, 22 Feb 2023 09:36:08 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 22 Feb 2023 09:36:10 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 01 Mar 2023 01:17:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 01:17:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 01:17:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Mar 2023 01:17:37 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Mon, 27 Mar 2023 20:18:06 GMT
ENV JAVA_VERSION=jdk-20+36
# Mon, 27 Mar 2023 20:18:28 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='980156d37580bd6fec142e02900497984e94c4b819a0c0eb7ce790bfc7c7d920';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='45dde71faf8cbb78fab3c976894259655c8d3de827347f23e0ebe5710921dded';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb6000faf47fffcda8caf01f60097d582728a6fffb6c1b85c8075c674f0c9281';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Mon, 27 Mar 2023 20:18:35 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 27 Mar 2023 20:18:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:afb26f3a2e2addc90e7fe9aa448a7bcb501afb7b8558e36a3ed2ac6de0d71842`  
		Last Modified: Tue, 28 Feb 2023 12:09:24 GMT  
		Size: 40.8 MB (40818261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16acb90c4c3d06f2c50b66a984d905d401528514e028f78a9ef301b58e2fc02b`  
		Last Modified: Wed, 01 Mar 2023 01:25:57 GMT  
		Size: 31.7 MB (31669606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b66d4cd4a793b65eec6c941cf55b37b95f5a859e06091ed8f041bc05f7912c`  
		Last Modified: Mon, 27 Mar 2023 20:21:17 GMT  
		Size: 202.0 MB (202000929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c858ef529f0075194b566e37323081a845d6ceb857b6374c7472a4c45279125e`  
		Last Modified: Mon, 27 Mar 2023 20:20:52 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
