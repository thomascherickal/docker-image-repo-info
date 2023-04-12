## `eclipse-temurin:17-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:49302f46f4e098a7012bb544e2150e74b054c3ffae91da9c84ec7b46fd282267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:5684dcbb2ad80cad256c3c837e82c943a96d27e07abb58793816dc35ee92d8ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113711618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b0d63d1b63e272154fb162af64de746e10e4d226a118e1a3fbef80e09d4a28`
-	Default Command: `["\/bin\/bash"]`

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
# Wed, 01 Mar 2023 00:15:09 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 01 Mar 2023 00:15:36 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 01 Mar 2023 00:15:37 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:e3604352dd07c282d84ebde1de602f1265bd9dfd15212dde9251d06d6272b36b`  
		Last Modified: Wed, 01 Mar 2023 00:20:19 GMT  
		Size: 46.9 MB (46934067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d7f47e430dc2f200c639ba89401337dc676cf01fdff938369de80732e40fe4`  
		Last Modified: Wed, 01 Mar 2023 00:20:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:cc3758c0e0cbd61e292f232933e8cfe85a3f6aab4a7020b3ea1564ff5a79ec39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.9 MB (111871906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71cbe8b6d37966404845896bdf218400f9041796e5784d42758ac574556f04ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Feb 2023 09:35:59 GMT
ADD file:0a0bf0de4876281b0338141009817b9753d8a4b377fb30d51800ad56d42735f3 in / 
# Wed, 22 Feb 2023 09:36:00 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 22 Feb 2023 09:36:00 GMT
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
# Wed, 22 Feb 2023 09:36:02 GMT
RUN rm -rf /var/log/*
# Wed, 22 Feb 2023 09:36:02 GMT
LABEL release=1793
# Wed, 22 Feb 2023 09:36:02 GMT
ADD file:aee30dec17fc14faad9acd396ee9d52fcfbde7619ab001f4f14e921d9dceb9bc in /root/buildinfo/content_manifests/ubi9-minimal-container-9.1.0-1793.json 
# Wed, 22 Feb 2023 09:36:02 GMT
ADD file:6767bc5857f7ee7adbfb0f1065508fa187b6a60b9f51af6f3844b305d151527d in /root/buildinfo/Dockerfile-ubi9-minimal-9.1.0-1793 
# Wed, 22 Feb 2023 09:36:02 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-02-22T09:23:20" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="befaf1f5ec7b874aef2651ee1384d51828504eb9" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.1.0-1793"
# Wed, 22 Feb 2023 09:36:03 GMT
RUN rm -f '/etc/yum.repos.d/repo-5af5d.repo' '/etc/yum.repos.d/repo-93eaf.repo'
# Wed, 22 Feb 2023 09:36:04 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 22 Feb 2023 09:36:06 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 01 Mar 2023 00:45:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 00:45:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 00:45:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Mar 2023 00:45:42 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Wed, 01 Mar 2023 00:46:47 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 01 Mar 2023 00:47:17 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 01 Mar 2023 00:47:18 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:1b885339e7dcfd6d72571e17b62a20ff54aad84d7242865fa4ca65a4ed648142`  
		Last Modified: Tue, 28 Feb 2023 12:09:12 GMT  
		Size: 36.1 MB (36138425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f664d3357ffe963399a90b6f2ac831d7fb19c6d9ed04aee823a95d92399218`  
		Last Modified: Wed, 01 Mar 2023 00:49:44 GMT  
		Size: 29.3 MB (29317629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68affc82534534783fee73e130a13567085a639cf47aa082a2f17af6682a892b`  
		Last Modified: Wed, 01 Mar 2023 00:51:32 GMT  
		Size: 46.4 MB (46415690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f4c53831a540bb413d0f9b0b457bd16e20f95e641ed6da7def602a6d9825bb`  
		Last Modified: Wed, 01 Mar 2023 00:51:27 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:8a6c9773ba2403827c9d379a09a3d644e4ae6a7c28ec7f152582bdc61d043440
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119280097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3fe1e67bb83a664097b64007e2292b36d4bbe97f410620dd837260c1035cbc`
-	Default Command: `["\/bin\/bash"]`

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
# Wed, 01 Mar 2023 01:20:01 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 01 Mar 2023 01:21:12 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 01 Mar 2023 01:21:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:420ea9b9141f063e9f6aab5833b36253902612faa1dfbbad2ad53c12b6127a36`  
		Last Modified: Wed, 01 Mar 2023 01:28:41 GMT  
		Size: 46.8 MB (46792070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29915a922458cf3e8a2b6d7b856ff09083e844b9e933237c37b32590b90e15e0`  
		Last Modified: Wed, 01 Mar 2023 01:28:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:6d2e5a94dc2258bf2d799eba20d4597934fa82ac608a72fa0c14855eef4e98dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114747948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6ac9d000e438c0e8b796c48a80f7fdcdee9412d323c36c61f5cf0e6cdecf90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 04 Apr 2023 13:09:15 GMT
ADD file:0d4be840bd5330d9d357aeb2d066c975d602f1d68d7de357091a0106f06a9cfa in / 
# Tue, 04 Apr 2023 13:09:31 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Tue, 04 Apr 2023 13:09:38 GMT
ADD file:214c1de395c24e4a86ef9a706069ef30a9e804c63f851c37c35655e16fea3ced in /tmp/tls-ca-bundle.pem 
# Tue, 04 Apr 2023 13:09:43 GMT
ADD multi:b69fbca1cffcb1fb28acb34486e2a3bc449bb345809fd618d7d6606c2a083b31 in /etc/yum.repos.d/ 
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL maintainer="Red Hat, Inc."
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.1.0"
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL io.openshift.expose-services=""
# Tue, 04 Apr 2023 13:09:43 GMT
LABEL io.openshift.tags="minimal rhel9"
# Tue, 04 Apr 2023 13:09:43 GMT
ENV container oci
# Tue, 04 Apr 2023 13:09:43 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 13:09:43 GMT
CMD ["/bin/bash"]
# Tue, 04 Apr 2023 13:09:50 GMT
RUN rm -rf /var/log/*
# Tue, 04 Apr 2023 13:09:50 GMT
LABEL release=1829
# Tue, 04 Apr 2023 13:09:55 GMT
ADD file:18dd601ebded76d5a9abaac93159d1334560e1639eafeb459de4e71c6d0887bd in /root/buildinfo/content_manifests/ubi9-minimal-container-9.1.0-1829.json 
# Tue, 04 Apr 2023 13:10:01 GMT
ADD file:a749effd5617ab084d7bd8726d7ac286e00c5c6dcd3604da315c4595ffb325f0 in /root/buildinfo/Dockerfile-ubi9-minimal-9.1.0-1829 
# Tue, 04 Apr 2023 13:10:01 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-04-04T12:58:00" "architecture"="s390x" "vcs-type"="git" "vcs-ref"="befaf1f5ec7b874aef2651ee1384d51828504eb9" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.1.0-1829"
# Tue, 04 Apr 2023 13:10:07 GMT
RUN rm -f '/etc/yum.repos.d/repo-6b42c.repo' '/etc/yum.repos.d/repo-8e12e.repo'
# Tue, 04 Apr 2023 13:10:11 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Tue, 04 Apr 2023 13:10:17 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 12 Apr 2023 17:57:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 17:57:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 17:57:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 12 Apr 2023 17:58:24 GMT
RUN microdnf install -y binutils tzdata openssl wget ca-certificates fontconfig glibc-langpack-en gzip tar     && microdnf clean all
# Wed, 12 Apr 2023 17:59:20 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 12 Apr 2023 17:59:57 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 12 Apr 2023 18:00:01 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:351bad2f1246888e886747c219e00a0507ae230fe5fd0a499b2f46c1aba439c8`  
		Last Modified: Wed, 12 Apr 2023 00:12:58 GMT  
		Size: 36.2 MB (36154357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21c097593b923dcfb4ed0f5d728f966d1161bdecd73280b10e2955d5172a784`  
		Last Modified: Wed, 12 Apr 2023 18:00:48 GMT  
		Size: 34.9 MB (34858948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25ba238f499b311bbbe5b8460ea52bd095c7125970ce465b7c9f4f8d0c62b31`  
		Last Modified: Wed, 12 Apr 2023 18:01:40 GMT  
		Size: 43.7 MB (43734483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beff022d892df18f71d42b403c2a4f4060e6f05d4c07cb844a0087fdc0472186`  
		Last Modified: Wed, 12 Apr 2023 18:01:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
