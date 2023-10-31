## `eclipse-temurin:21-jdk-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:0f23b4b542d2027ab7e59a0dc26fd5a445537c054ef5219ea334a52368e2cb9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:21-jdk-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:0454b270e68115dca18208ef8833b9d0166792dd50895ea4c14c09e5d690e628
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.4 MB (224354758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df2f3db70ee8027db9e681d88d24815ff31e7f699832cb2eaf387c51aac1220`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

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
# Mon, 30 Oct 2023 23:30:07 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:30:15 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='e184dc29a6712c1f78754ab36fb48866583665fa345324f1a79e569c064f95e9';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_aarch64_linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1a6fa8abda4c5caed915cfbeeb176e7fbd12eb6b222f26e290ee45808b529aa1';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_linux_hotspot_21.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9574828ef3d735a25404ced82e09bf20e1614f7d6403956002de9cfbfcb8638f';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_ppc64le_linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:30:18 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:30:18 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:30:18 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 30 Oct 2023 23:30:18 GMT
CMD ["jshell"]
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
	-	`sha256:4469af3cacb7d9b64e8d921642fab07f28dccf872f8eacd90bcd93a6b8f76c19`  
		Last Modified: Mon, 30 Oct 2023 23:39:29 GMT  
		Size: 158.6 MB (158633026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae8e530e63f4ed9e0da35021af7f42f57bb98180e047a7b11ff8c263e6360`  
		Last Modified: Mon, 30 Oct 2023 23:39:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ed3bc9ee933253a7a52421183cbe06d6d37354edb1953cd6fc4cd47c329f0f`  
		Last Modified: Mon, 30 Oct 2023 23:39:16 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:21-jdk-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:f19fcbf86bd34b425c8d1df8ac507403dc181d22293a1f5b8a7427b165164df9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221301387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e608dba55022e641a2236d9f333700590840fbdfc6f6acc06d84564313f704a`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

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
# Mon, 30 Oct 2023 23:46:20 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:46:28 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='e184dc29a6712c1f78754ab36fb48866583665fa345324f1a79e569c064f95e9';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_aarch64_linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1a6fa8abda4c5caed915cfbeeb176e7fbd12eb6b222f26e290ee45808b529aa1';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_linux_hotspot_21.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9574828ef3d735a25404ced82e09bf20e1614f7d6403956002de9cfbfcb8638f';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_ppc64le_linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:46:31 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:46:31 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:46:31 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 30 Oct 2023 23:46:31 GMT
CMD ["jshell"]
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
	-	`sha256:97c8fdfdcc7a84d280cecdd274f569d03ce5aa99cfd50e6b27a91bc41db65108`  
		Last Modified: Mon, 30 Oct 2023 23:53:40 GMT  
		Size: 156.9 MB (156875731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dead7ea359fddaf182c80cda73909a513743f8cea9a2f64f0b6d2d4f854a56`  
		Last Modified: Mon, 30 Oct 2023 23:53:30 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ef787b35e9eeb63f62a2323e695b2aeffaa765df53b96308c5229b93926ba`  
		Last Modified: Mon, 30 Oct 2023 23:53:30 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:21-jdk-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:25fbad94c99a7830c8cd291a910aa208cb40149c74722d847d363ea8057f7a3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230936402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40701c765058999c24a59d1babe417d2a4f65633c8876ba855f21beabf2df956`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

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
# Mon, 30 Oct 2023 23:27:45 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:27:56 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='e184dc29a6712c1f78754ab36fb48866583665fa345324f1a79e569c064f95e9';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_aarch64_linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1a6fa8abda4c5caed915cfbeeb176e7fbd12eb6b222f26e290ee45808b529aa1';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_linux_hotspot_21.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9574828ef3d735a25404ced82e09bf20e1614f7d6403956002de9cfbfcb8638f';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_ppc64le_linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:28:01 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:28:01 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:28:02 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 30 Oct 2023 23:28:02 GMT
CMD ["jshell"]
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
	-	`sha256:c3ccda07c8f27b0f1ec85ec10e403175b2ef29b68aa517f3a50a6429593a1cc1`  
		Last Modified: Mon, 30 Oct 2023 23:35:48 GMT  
		Size: 158.2 MB (158238126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d043fd45fd1b04196f8e56b49abca6470748fcbe2ced5277f890cc282e2f012f`  
		Last Modified: Mon, 30 Oct 2023 23:35:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacf387248c3d01165c7150133658a19e1c1c05a43e5c1619900f7a4ac2b6a6f`  
		Last Modified: Mon, 30 Oct 2023 23:35:34 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
