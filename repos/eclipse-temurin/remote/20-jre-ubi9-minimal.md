## `eclipse-temurin:20-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:4f232f8f1cb36a1e8c8023d63c952a07cdeacab3312e35cdfba913b0b9f078be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:20-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:df75eee479e83d97ad4c8ff8c05c2c2d281657752ba6312a8fbf70ba817835e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116861544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4f122cedfdb1b8e638859a745cf69cccd519a54946cd8f5518bbc022d1bd2d`
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
# Mon, 27 Mar 2023 20:24:55 GMT
ENV JAVA_VERSION=jdk-20+36
# Mon, 27 Mar 2023 20:25:28 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='b226140b8efacf21d256203cc8f919549e295cb9bac88b24c15fb8e53a66b545';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a1c5a16d5a438ce7da4563cd51ff6778cdf62331c00a3096ab2388a916e076d2';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f41be99b1fd21873b0fa1436bb206119706922e9c4b32298538faf3d1b632a72';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Mon, 27 Mar 2023 20:25:29 GMT
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
	-	`sha256:44525eaf0644532823d14c2f2ee4ebbc526f83df9ab88219670f278ebbf2ebf3`  
		Last Modified: Mon, 27 Mar 2023 20:28:30 GMT  
		Size: 50.1 MB (50083992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e26ee3942331bdcf4c4fae5908348e96339bffb01822d998ef35e971a038657`  
		Last Modified: Mon, 27 Mar 2023 20:28:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:5ce6441a37844f711cb6368357c4008d0672f55eedb06216438a8adf7e01d13d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114804784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd0cc77556ffa8d8f9c8011f0aa92b10ec2210b8567a7d68b316e9b3f4ca30a`
-	Default Command: `["\/bin\/bash"]`

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
# Wed, 12 Apr 2023 21:02:53 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='b226140b8efacf21d256203cc8f919549e295cb9bac88b24c15fb8e53a66b545';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a1c5a16d5a438ce7da4563cd51ff6778cdf62331c00a3096ab2388a916e076d2';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f41be99b1fd21873b0fa1436bb206119706922e9c4b32298538faf3d1b632a72';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 12 Apr 2023 21:02:54 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:8193cc7349604fb56cd317c0127d8baeb658c9518ce2ac8d7ba21a4d10ebdec8`  
		Last Modified: Wed, 12 Apr 2023 21:06:04 GMT  
		Size: 49.3 MB (49304140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c849f4f325457075fff7d75599951729750be4cf80e9dc40b4fc3f5cb6e8d`  
		Last Modified: Wed, 12 Apr 2023 21:05:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:6647d7b7efabcf2aa48d5ab904a967c8ff0acc3d309cd1ac0f9471ba95f03b17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122333979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981ae24a9edf43f4a17136dadfc5eb1ffa573c8afbfc836ef45b03081ac2c1f2`
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
# Mon, 27 Mar 2023 20:18:06 GMT
ENV JAVA_VERSION=jdk-20+36
# Mon, 27 Mar 2023 20:19:03 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='b226140b8efacf21d256203cc8f919549e295cb9bac88b24c15fb8e53a66b545';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a1c5a16d5a438ce7da4563cd51ff6778cdf62331c00a3096ab2388a916e076d2';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f41be99b1fd21873b0fa1436bb206119706922e9c4b32298538faf3d1b632a72';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Mon, 27 Mar 2023 20:19:06 GMT
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
	-	`sha256:6a361b42ce6c348c91995f8ca9b831a1f4450dd64a40b2c3ef2efc70cdc6bbe8`  
		Last Modified: Mon, 27 Mar 2023 20:22:04 GMT  
		Size: 49.8 MB (49845952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da3239254535c92f50db146fadb19b49b183453b20510dea62f48657fa1e5d1`  
		Last Modified: Mon, 27 Mar 2023 20:21:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
