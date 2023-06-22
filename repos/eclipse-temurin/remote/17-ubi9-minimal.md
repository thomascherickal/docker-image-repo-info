## `eclipse-temurin:17-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:2c7c10247a3806fb282d434a96583ccc56ac2c1c86c488ed3d84cc95607b2ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:17-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:2d5b228568afdccb76f87f969ec915826fd81f6c4502ff482694052cfbb84f43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258287498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df872e3540deb08ffda05302f14cc9403248653ebd76e6cec76d338989e4e13f`
-	Default Command: `["jshell"]`

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
# Thu, 22 Jun 2023 01:09:47 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:09:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 22 Jun 2023 01:09:50 GMT
CMD ["jshell"]
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
	-	`sha256:f4efb52b26e06b61a13808d3ece8abc061b2c55cdc570868a6c14e3638dc5873`  
		Last Modified: Thu, 22 Jun 2023 01:13:13 GMT  
		Size: 192.6 MB (192589216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3097d81781c62ea7a67d3694d8d32a33fe94c22b174bb9abe10e06bb25b372`  
		Last Modified: Thu, 22 Jun 2023 01:13:00 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:541c457de1d9ee2d41681c95e138129bc72024ca4cfc91c03780c3a8b4b2df81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.8 MB (255829703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0180cd9ce84426c50dfbdd28a9406edbe3a47572662edb3529e5cac523ebf290`
-	Default Command: `["jshell"]`

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
# Thu, 22 Jun 2023 01:23:32 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:23:35 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 22 Jun 2023 01:23:35 GMT
CMD ["jshell"]
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
	-	`sha256:cb56aa247287b810221c0c31927c61f66b44ae36b62a630f03911e00792b3b43`  
		Last Modified: Thu, 22 Jun 2023 01:26:36 GMT  
		Size: 191.4 MB (191395726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fefbcee872cd35b89c99c27c2cca296a1e3c3dd4193e2caa760601f31ef719d`  
		Last Modified: Thu, 22 Jun 2023 01:26:26 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:624a9947b2c9110691a7949f55fc1e57865b4f69b750cce4c8019c298c7a4aa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.7 MB (264661604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0237db973cc4ac178dc23df56c962e575697a15ed7bfa794de5945eddbe1e0`
-	Default Command: `["jshell"]`

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
# Thu, 22 Jun 2023 01:17:52 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 01:18:00 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 22 Jun 2023 01:18:00 GMT
CMD ["jshell"]
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
	-	`sha256:b7331b6a45c0f3cd5fb8efc5855082808b9a3ec6d276c2fc3739d7655f12a01a`  
		Last Modified: Thu, 22 Jun 2023 01:21:12 GMT  
		Size: 192.0 MB (191976808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31eb5ee076cb6101635448449b73472b95962b87c963f285feb15ba3b6d4ddda`  
		Last Modified: Thu, 22 Jun 2023 01:20:48 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:508e13835f4b8a0cfbf507bf20ba91b029f4e0ae9874dce63ed954334ab151f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244406609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06508cfb439bf408b9f6246672c47ac3d7833abbbb8ea020985697b031587725`
-	Default Command: `["jshell"]`

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
# Thu, 22 Jun 2023 10:52:38 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 22 Jun 2023 10:52:44 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 22 Jun 2023 10:52:45 GMT
CMD ["jshell"]
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
	-	`sha256:fa936366e1993e2d79e204da57f3b365d9b82c1f77dc444b88f72a779952df2f`  
		Last Modified: Thu, 22 Jun 2023 10:54:44 GMT  
		Size: 180.4 MB (180350448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b33fe80db17a828d1c282aa0ae7b9c12f5b59d170795abdbf15f44b57d7c6d`  
		Last Modified: Thu, 22 Jun 2023 10:54:31 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
