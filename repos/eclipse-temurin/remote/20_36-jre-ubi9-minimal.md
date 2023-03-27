## `eclipse-temurin:20_36-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:ddd15d3831770ff7f5e69528b1f988b560a9679a8b6dae28aa18379ed60be9b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `eclipse-temurin:20_36-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:ec1e6f153ce6de19ca6f94fc0f5a920843ff74c3dc88c72beb377f6aaea6b64e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114760353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c1892e303aeffae89fca90afbbdd74c852a14d0a2d5bf2f8b778fe396ff2ec`
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
# Mon, 27 Mar 2023 19:41:13 GMT
ENV JAVA_VERSION=jdk-20+36
# Mon, 27 Mar 2023 19:41:37 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='b226140b8efacf21d256203cc8f919549e295cb9bac88b24c15fb8e53a66b545';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a1c5a16d5a438ce7da4563cd51ff6778cdf62331c00a3096ab2388a916e076d2';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f41be99b1fd21873b0fa1436bb206119706922e9c4b32298538faf3d1b632a72';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Mon, 27 Mar 2023 19:41:38 GMT
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
	-	`sha256:fe01dc514cd7567a8641ba37abe48bf54d01ca1d714565a2f80fd1869eb16fa8`  
		Last Modified: Mon, 27 Mar 2023 19:43:54 GMT  
		Size: 49.3 MB (49304139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c83e8b612e6f1b2fe21b187a2cb9ff0dcc21584cac238c2d0aa501cf8ba4047`  
		Last Modified: Mon, 27 Mar 2023 19:43:48 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
