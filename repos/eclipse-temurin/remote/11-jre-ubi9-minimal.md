## `eclipse-temurin:11-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:e7bbbc04c72fc30b4ce1444509b94547fc556b7f4f8a0d7cadc151d496ee2c6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:914d7524fce7d51638db193efebb1a5de486acbfaeb0e5a5ee515df80d6a36fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109795745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:584296af283ebdbd4a28b98b00b6b842cf4fd9080ba19466637a6f3949e75b2f`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 18 Oct 2023 11:43:37 GMT
ADD file:139424fc60c0a17394da68faf4af3a17c9e959b6a1ce74c5b53ffc959145a63c in / 
# Wed, 18 Oct 2023 11:43:38 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 11:43:38 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 11:43:38 GMT
ADD multi:eed63f5f84efa377cb20d8bc2a3294d6aeffff59ee5380d49f1903b9673516dd in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 11:43:38 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 18 Oct 2023 11:43:38 GMT
ENV container oci
# Wed, 18 Oct 2023 11:43:38 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 11:43:38 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 11:43:38 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 11:43:39 GMT
ADD file:d4e564939c7991d70e1c5392b02502c604ec36a1612a39fc922b8bb32a567932 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-750.1697625013.json 
# Wed, 18 Oct 2023 11:43:39 GMT
ADD file:7aa78ccab5aa351a2b340ceba6ac1dad0988268ffec2b6ff113734e516c775f9 in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-750.1697625013 
# Wed, 18 Oct 2023 11:43:39 GMT
LABEL "release"="750.1697625013" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:30:28" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-750.1697625013"
# Wed, 18 Oct 2023 11:43:39 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460177-f3ccb.repo' '/etc/yum.repos.d/gitweb-a7836.repo'
# Wed, 18 Oct 2023 11:43:40 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 11:43:41 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 20 Oct 2023 00:05:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 20 Oct 2023 00:05:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Oct 2023 00:05:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:25:34 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Mon, 30 Oct 2023 23:25:34 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:26:25 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:26:25 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:26:26 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:26:26 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:2f5211d9dccf1de31345273282bf9a4f2a32341a7352b0435155277e54fc0cd1`  
		Last Modified: Thu, 19 Oct 2023 00:06:30 GMT  
		Size: 37.9 MB (37862118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0b0f58ef9011e018fcffd443ef584a45e1560ae51a4cafeb8d18134434198`  
		Last Modified: Mon, 30 Oct 2023 23:33:41 GMT  
		Size: 27.9 MB (27858727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411ec1caeda829b596e4dbb6320457d38a17853af87419cf4cf4f061ce86ffdf`  
		Last Modified: Mon, 30 Oct 2023 23:35:08 GMT  
		Size: 44.1 MB (44074029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6b0fd525e30200599fe98ab3ad97591d19f3b06483eedf05ceb45025e3851a`  
		Last Modified: Mon, 30 Oct 2023 23:35:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2f10eba3f55265b970f795d41c575fed64ac02074bc1d1c91ef96eebc60eb5`  
		Last Modified: Mon, 30 Oct 2023 23:35:02 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:d951ef1e4c1e169f040089e12b0451e06a73758c0f57c623027503553d185d7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106833312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233daefb77837d0e93b3a7ae6d9f58101204a17b476667272e8f96935712a7e8`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 18 Oct 2023 11:43:35 GMT
ADD file:e691ccb76303edd2d82b816fda94f210ce903198b687214308ff27960f8efe7e in / 
# Wed, 18 Oct 2023 11:43:36 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 11:43:36 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 11:43:36 GMT
ADD multi:eed63f5f84efa377cb20d8bc2a3294d6aeffff59ee5380d49f1903b9673516dd in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 11:43:36 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 18 Oct 2023 11:43:36 GMT
ENV container oci
# Wed, 18 Oct 2023 11:43:36 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 11:43:36 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 11:43:37 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 11:43:37 GMT
ADD file:4a13e96a4ab8bba5cc4ea503ebfefc7c94cec53a788f71e4c40f2e83ae23331e in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-750.1697625013.json 
# Wed, 18 Oct 2023 11:43:37 GMT
ADD file:07283ec4d328adf575cda694a931e0281866cd74c6c9a6fde161775cb6be8ddb in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-750.1697625013 
# Wed, 18 Oct 2023 11:43:37 GMT
LABEL "release"="750.1697625013" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:30:28" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-750.1697625013"
# Wed, 18 Oct 2023 11:43:39 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460177-f3ccb.repo' '/etc/yum.repos.d/gitweb-a7836.repo'
# Wed, 18 Oct 2023 11:43:40 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 11:43:41 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 20 Oct 2023 02:32:21 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 20 Oct 2023 02:32:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Oct 2023 02:32:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:42:37 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Mon, 30 Oct 2023 23:42:37 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:43:12 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:43:13 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:43:13 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:43:13 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:472e9d218c02b84dcd7425232d8b1ac2928602de2de0efc01a7360d1d42bf2f6`  
		Last Modified: Thu, 19 Oct 2023 00:06:36 GMT  
		Size: 36.1 MB (36135743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb82435762e41b1e7db9a145dd1499d6687e27ef7fbc3b1910eadeb66c25f19`  
		Last Modified: Mon, 30 Oct 2023 23:49:06 GMT  
		Size: 28.3 MB (28289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1768469ca08a6b43708cb1573fa5b68ea91543bc3644d1bd184106b27737955c`  
		Last Modified: Mon, 30 Oct 2023 23:50:10 GMT  
		Size: 42.4 MB (42407672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11bbc5f390eb3fdf94aebacdfb541e134cfcc0f7edb3ddc6f885b10a00672e8`  
		Last Modified: Mon, 30 Oct 2023 23:50:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751f09cff6874baa66050714453c2d2aa8847bd7f933a7716fec3df1b94971b`  
		Last Modified: Mon, 30 Oct 2023 23:50:05 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:35e66ea6d144afde48fd319f3b78cfe2464284bcad3ffc1769d1ad14848d0b84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112244076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da5f4a113d13c9eec1e70d5d49fae6b74392a3136d9d138c465c92325ffa172`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 18 Oct 2023 11:43:39 GMT
ADD file:38ff720f4bd0542e52135d7ca8462094c1d1a25eb1abf1c9ca6eb62629b8fa8b in / 
# Wed, 18 Oct 2023 11:43:41 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 11:43:41 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 11:43:41 GMT
ADD multi:eed63f5f84efa377cb20d8bc2a3294d6aeffff59ee5380d49f1903b9673516dd in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 11:43:41 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 18 Oct 2023 11:43:41 GMT
ENV container oci
# Wed, 18 Oct 2023 11:43:41 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 11:43:41 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 11:43:42 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 11:43:43 GMT
ADD file:51bb6dd1dd93dba3254f6fc74f978bac7f55ca7d4182a71200a400302bb24286 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-750.1697625013.json 
# Wed, 18 Oct 2023 11:43:43 GMT
ADD file:8f43dd15756179218863800cd8e3e9eaf62665a86818b2b3df7d986f62a788db in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-750.1697625013 
# Wed, 18 Oct 2023 11:43:43 GMT
LABEL "release"="750.1697625013" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:30:28" "architecture"="ppc64le" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-750.1697625013"
# Wed, 18 Oct 2023 11:43:44 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460177-f3ccb.repo' '/etc/yum.repos.d/gitweb-a7836.repo'
# Wed, 18 Oct 2023 11:43:46 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 11:43:48 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 20 Oct 2023 01:46:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 20 Oct 2023 01:46:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Oct 2023 01:46:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:21:30 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Mon, 30 Oct 2023 23:21:32 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:22:42 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:22:45 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:22:45 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:22:46 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:56c49f9b2030400a6f12e76696bcf5a933a6bc310009c4f802ef70e51862c56a`  
		Last Modified: Thu, 19 Oct 2023 00:06:44 GMT  
		Size: 42.3 MB (42278290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b743d7c769ce21e9022904a927acfd5ea0a675de92d0681d66451dec48acad`  
		Last Modified: Mon, 30 Oct 2023 23:30:50 GMT  
		Size: 30.4 MB (30419100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c833eb73024f1dc959767d6ec37dacf79866131c7772b21e2199d0dab373bc`  
		Last Modified: Mon, 30 Oct 2023 23:32:03 GMT  
		Size: 39.5 MB (39545818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c4133f5629fd6d77a703c807197f505cbd66fcacbb4558e84060012579d60`  
		Last Modified: Mon, 30 Oct 2023 23:31:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e0dbf9a1324eda0064f6c84c46ea4bcfc809af1b6f7687691056dc073d86e`  
		Last Modified: Mon, 30 Oct 2023 23:31:57 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:2295dd9506884ee2ee16943e76516116e51192716ab1c94baf9a9c82ee466fc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101760701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acc7fcb27e72754d36dff14b63f41b8f9fd34755227f5bdbfda2e3b1e9f8f8b7`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 18 Oct 2023 11:43:40 GMT
ADD file:f95119de615b06c72c8f5c9ec6610dddec6d1a41dcc4be1003c25a1c57f97d37 in / 
# Wed, 18 Oct 2023 11:43:41 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 18 Oct 2023 11:43:42 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 18 Oct 2023 11:43:42 GMT
ADD multi:eed63f5f84efa377cb20d8bc2a3294d6aeffff59ee5380d49f1903b9673516dd in /etc/yum.repos.d/ 
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.2"
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL io.openshift.expose-services=""
# Wed, 18 Oct 2023 11:43:42 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 18 Oct 2023 11:43:42 GMT
ENV container oci
# Wed, 18 Oct 2023 11:43:42 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 11:43:42 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 11:43:43 GMT
RUN rm -rf /var/log/*
# Wed, 18 Oct 2023 11:43:44 GMT
ADD file:4bf9e4d77f4210d89b4696aef310d06b423776e3eba420f72e29a86250b3fc18 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.2-750.1697625013.json 
# Wed, 18 Oct 2023 11:43:44 GMT
ADD file:7f00e3fef3b2fb5119c5c04958a23a8f6c72857ed02cbeac858ef06bb6a48f4e in /root/buildinfo/Dockerfile-ubi9-minimal-9.2-750.1697625013 
# Wed, 18 Oct 2023 11:43:44 GMT
LABEL "release"="750.1697625013" "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-10-18T11:30:28" "architecture"="s390x" "vcs-type"="git" "vcs-ref"="7ef59505f75bf0c11c8d3addefebee5ceaaf4c41" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.2-750.1697625013"
# Wed, 18 Oct 2023 11:43:45 GMT
RUN rm -f '/etc/yum.repos.d/odcs-2460177-f3ccb.repo' '/etc/yum.repos.d/gitweb-a7836.repo'
# Wed, 18 Oct 2023 11:43:46 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 18 Oct 2023 11:43:48 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 20 Oct 2023 01:39:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 20 Oct 2023 01:39:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Oct 2023 01:39:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:24:53 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Mon, 30 Oct 2023 23:24:54 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:25:45 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:25:47 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:25:47 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:25:47 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:c6c38ccb2ffffe0f49cf030245259cca431b2ff0dd58896de36b676e5cc2801d`  
		Last Modified: Thu, 19 Oct 2023 00:06:50 GMT  
		Size: 36.1 MB (36109625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e184afd59192e217fac5ab0fa025cd4af5b562e36892bc47eb7db49971a18`  
		Last Modified: Mon, 30 Oct 2023 23:29:31 GMT  
		Size: 27.9 MB (27911148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a804b1e3baabc1eaf3f432a5db305d902062d5e7dc13b6709a34237275facd`  
		Last Modified: Mon, 30 Oct 2023 23:30:15 GMT  
		Size: 37.7 MB (37739057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6e386b23d29da2274fb651dc99ba4118ed2870d7565bb3a6858e145a88e93`  
		Last Modified: Mon, 30 Oct 2023 23:30:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6ed1bfa1f6ce010f0be6e82c9ffc272c033afb375650258c5c76415eece528`  
		Last Modified: Mon, 30 Oct 2023 23:30:10 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
