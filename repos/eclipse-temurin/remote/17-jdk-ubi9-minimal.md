## `eclipse-temurin:17-jdk-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:f35c239527b6926913c5971aa856026a622e7c1027ad5c316a1fc5c971d14eda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:17-jdk-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:fc68c5f484651aa22d221a25836d7aeaab2056becc03bc59cdbd539ef4b00635
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259217240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f427980d587130fb722e122be358fa631ab7636dca08752faec656cdd76f60d`
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
# Wed, 01 Mar 2023 00:15:09 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 01 Mar 2023 00:15:17 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 01 Mar 2023 00:15:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 01 Mar 2023 00:15:20 GMT
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
	-	`sha256:d01c3a97db9ac43a63e34bef94bc3624c58bd42fa3d8c699a1163aa929c12244`  
		Last Modified: Wed, 01 Mar 2023 00:19:57 GMT  
		Size: 192.4 MB (192439670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca82213befeb789d3f3a16cb690df7c3cc141b44cb0e7e4fc7cc41b215b5bf3`  
		Last Modified: Wed, 01 Mar 2023 00:19:43 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:0e21be8253054578cfb3758bb53f2fbd2d6aa4ae4ffde2b7b84b8edc06c87a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.8 MB (256766056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5e36aebb95fbfdc3940005e23eda4819b12f83341c6c62162e15654be4dbc3`
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
# Wed, 12 Apr 2023 21:02:09 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 12 Apr 2023 21:02:17 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 12 Apr 2023 21:02:21 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 12 Apr 2023 21:02:21 GMT
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
	-	`sha256:dfc035cf16a63b4fa83e5f6054310eb1f40f13f339425d4d3f0b71619b18297f`  
		Last Modified: Wed, 12 Apr 2023 21:05:09 GMT  
		Size: 191.3 MB (191265396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d49874288d3e1492a2f4c1e7b7f9de3d70b2b005e478ca67f6bdbd5817604f`  
		Last Modified: Wed, 12 Apr 2023 21:04:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:fc739c8727072f0f0d35186ed97330f0a17e3a9380d20fb759bd2f2a7894816e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.3 MB (264306888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0237cb499c277e92477d0bf0229e93171abcccd380ec479ed792ea2d746793`
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
# Wed, 01 Mar 2023 01:20:01 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 01 Mar 2023 01:20:36 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 01 Mar 2023 01:20:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 01 Mar 2023 01:20:44 GMT
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
	-	`sha256:c7146458c1aa5314a86c1adb48dc92ca16126f9686c9e55429873d49d481e9cd`  
		Last Modified: Wed, 01 Mar 2023 01:28:11 GMT  
		Size: 191.8 MB (191818841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938f1c778a240000111d1359164708cdefb7199255a0cc5782a5c1785dab3d62`  
		Last Modified: Wed, 01 Mar 2023 01:27:47 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:f9d3ea1f00bc3efb09ff6aacd3b540d41e7238c98f884a429903db6633f1d017
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.3 MB (251292244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72be2d215631a33b0e191c8b8ba46ba173777b8542c0b4220dd35d5c6296b027`
-	Default Command: `["jshell"]`

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
# Wed, 12 Apr 2023 17:59:30 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 12 Apr 2023 17:59:39 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 12 Apr 2023 17:59:39 GMT
CMD ["jshell"]
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
	-	`sha256:83da14ce204826664aa9745b73c1327cf7ea4d62cf9357fd0cbb4a48b97db675`  
		Last Modified: Wed, 12 Apr 2023 18:01:26 GMT  
		Size: 180.3 MB (180278763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f584c54f18a92bbf8bddcf53df03310ae4a1036e180314a86b80c49775a94b`  
		Last Modified: Wed, 12 Apr 2023 18:01:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
