## `eclipse-temurin:17-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:8c7101908bb8c10c7d592802eab9887200899d9c76e1954c346381cf21fd4d7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:7614a3be6a33cf0ed8e31d61694c861e4a731a63665d088e19e1f3096d3fd87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112699636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c059ecf4bb5a6f314dc85acf477a5f39daf20b4975aaad3c7eec11ad6f180c1`
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
# Thu, 22 Jun 2023 01:09:40 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 22 Jun 2023 01:10:06 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:10:07 GMT
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
	-	`sha256:5e95f1a6d1ec791f5939f7cd7239a8c814d5897bc598e8e790adfd4ec0a098d2`  
		Last Modified: Thu, 22 Jun 2023 01:13:31 GMT  
		Size: 47.0 MB (47001373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee702ef5646877d7b7126d41e6519d22ee160ed1a8dac99c94f6a131139eb7e`  
		Last Modified: Thu, 22 Jun 2023 01:13:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:cd92111db415567bcf0698a81b99775283e9ccc9acb53b8b0918b965424e9ff3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110919198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c54d0c3c64cf12128608a17de7b5207438f124eaf0cca69109d2ccef0eaea22`
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
# Thu, 22 Jun 2023 01:23:23 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 22 Jun 2023 01:23:47 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:23:48 GMT
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
	-	`sha256:ce7e4e5e9bed4b2dc5ea2cee7c08f9a6ba7ff705d2986d93f59235436eef78c0`  
		Last Modified: Thu, 22 Jun 2023 01:26:55 GMT  
		Size: 46.5 MB (46485239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3d3a4f8934d68654e640992ad6696e9825503888b45aabb88a6ae51c6ee0a`  
		Last Modified: Thu, 22 Jun 2023 01:26:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:ece1eff3a37ad54d161f885ca1e96073f0e7a60fd6114c5692219d2cae0b6d1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119562262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9753d07a291de164261f0bd169ba2201a05bad2d1711ae257b0435fafeed23`
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
# Thu, 22 Jun 2023 01:17:34 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 22 Jun 2023 01:18:18 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:18:21 GMT
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
	-	`sha256:e1c7274b56da56bdcade868c809ba4a1d157e8bfe4c242d7881c4958e8429fb4`  
		Last Modified: Thu, 22 Jun 2023 01:21:37 GMT  
		Size: 46.9 MB (46877483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e199b8673428eecea02b21b651c3e63678911b37b67a43e1b1f196aa19cd5568`  
		Last Modified: Thu, 22 Jun 2023 01:21:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:14a8eae350ffdd750439c0b8626b133321d905cd536837aa09b89d66d7b33523
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107820618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308e89fec653deae396576308f48d46e1c6b6dc65f894cc3ac7207e311f148ce`
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
# Thu, 22 Jun 2023 10:52:28 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 22 Jun 2023 10:53:07 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 10:53:10 GMT
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
	-	`sha256:f47e0a98eb7a1aaae4d3abc4d219e60d8999d46c2126a9e36cd0b754ff512a0d`  
		Last Modified: Thu, 22 Jun 2023 10:55:00 GMT  
		Size: 43.8 MB (43764476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36a7e1d461006bc6a667bc1200eee9e072fd5017add59961f406f7523e24fbb`  
		Last Modified: Thu, 22 Jun 2023 10:54:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
