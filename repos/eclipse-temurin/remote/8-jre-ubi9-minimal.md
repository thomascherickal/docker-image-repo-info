## `eclipse-temurin:8-jre-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:f4de866c60d88a7e6f26274515eb0af245c76792b6bd8e5757d887058495a375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:8-jre-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:ce4364b464d73c4e2c03efb9b4c877830c29895f378c8ad5df4a56c5aec70456
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 MB (107467237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c9253a9e47c0d03a5468e459371ffdc31d8bb8924ed16ebb41ba3c16184bcf`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 01 Nov 2023 01:47:47 GMT
ADD file:2301f31446233cc7f48641aa49d559ff35153508e83f58b40f8a5e6bf4e6d673 in / 
# Wed, 01 Nov 2023 01:47:48 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 01 Nov 2023 01:47:48 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 01 Nov 2023 01:47:48 GMT
ADD multi:de99ba40d34adfc554e955bb344f3584a5587f990f2c5ac525d44349cf2c6f4b in /etc/yum.repos.d/ 
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.3"
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL io.openshift.expose-services=""
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 01 Nov 2023 01:47:48 GMT
ENV container oci
# Wed, 01 Nov 2023 01:47:48 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 01:47:48 GMT
CMD ["/bin/bash"]
# Wed, 01 Nov 2023 01:47:49 GMT
RUN rm -rf /var/log/*
# Wed, 01 Nov 2023 01:47:49 GMT
LABEL release=1361
# Wed, 01 Nov 2023 01:47:49 GMT
ADD file:6b0d494705c61a25b2f83a36df94f106de9fceebd0457f115320d3125d055e47 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.3-1361.json 
# Wed, 01 Nov 2023 01:47:49 GMT
ADD file:4c1b0ed13af21a336c482e4f480745c59c966457da4322ac65a4bb8495f1d801 in /root/buildinfo/Dockerfile-ubi9-minimal-9.3-1361 
# Wed, 01 Nov 2023 01:47:49 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-01T01:38:36" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="e8510c65a9be4b0635372fd09bee126ce7e08bc7" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.3-1361"
# Wed, 01 Nov 2023 01:47:49 GMT
RUN rm -f '/etc/yum.repos.d/repo-7e938.repo' '/etc/yum.repos.d/repo-2aab0.repo'
# Wed, 01 Nov 2023 01:47:50 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 01 Nov 2023 01:47:51 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 08 Nov 2023 01:10:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 08 Nov 2023 01:10:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Nov 2023 01:10:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Nov 2023 01:10:46 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Wed, 08 Nov 2023 01:10:46 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 08 Nov 2023 01:11:08 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:11:09 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Wed, 08 Nov 2023 01:11:09 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:11:09 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:e53f59cdb1fb57d78c0763b14f461843605f1319da9cf08c375ead2a80772112`  
		Last Modified: Tue, 07 Nov 2023 12:07:42 GMT  
		Size: 37.7 MB (37730907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0a5c57bc6845f649323f1aada4f22f4ce5cba3894b1d0d1e230f5c437107c9`  
		Last Modified: Wed, 08 Nov 2023 01:14:25 GMT  
		Size: 27.9 MB (27880623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b5b5d2064584cc7b74fc1021f64073066a2bda36f34f5035ab259a6cfe89d5`  
		Last Modified: Wed, 08 Nov 2023 01:14:52 GMT  
		Size: 41.9 MB (41854836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa66bec95dd9083e3fda1bbfb939ef3a14ef422bce10a684a2237bab0c3cc1b`  
		Last Modified: Wed, 08 Nov 2023 01:14:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc5f6ffe98f34aa39fad47d0a8a59a8f2a118d20f494840b94e72b816686fa3`  
		Last Modified: Wed, 08 Nov 2023 01:14:47 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:05093590f59f2a8965c452a1876d46935857ef98bf06f089d71af39e982f7b05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105191350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65bd8600de6b13d1a427981d223b7e03555ae5e1ec9c0346af09b8ffd6dc9ca`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 01 Nov 2023 01:47:46 GMT
ADD file:67879f44eff6023f7e40b96450fc9e266c67d79a6657493c7d371e09b766fa76 in / 
# Wed, 01 Nov 2023 01:47:47 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 01 Nov 2023 01:47:47 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 01 Nov 2023 01:47:48 GMT
ADD multi:de99ba40d34adfc554e955bb344f3584a5587f990f2c5ac525d44349cf2c6f4b in /etc/yum.repos.d/ 
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.3"
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL io.openshift.expose-services=""
# Wed, 01 Nov 2023 01:47:48 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 01 Nov 2023 01:47:48 GMT
ENV container oci
# Wed, 01 Nov 2023 01:47:48 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 01:47:48 GMT
CMD ["/bin/bash"]
# Wed, 01 Nov 2023 01:47:49 GMT
RUN rm -rf /var/log/*
# Wed, 01 Nov 2023 01:47:49 GMT
LABEL release=1361
# Wed, 01 Nov 2023 01:47:49 GMT
ADD file:74ec779ce6a1057d3820203476542b91d590a11316bacae3be519e6bcff6f28e in /root/buildinfo/content_manifests/ubi9-minimal-container-9.3-1361.json 
# Wed, 01 Nov 2023 01:47:49 GMT
ADD file:7f8ab01133336752c788dc0a8553c9aba5741ca967a2245cb5c8f340c45ca6fb in /root/buildinfo/Dockerfile-ubi9-minimal-9.3-1361 
# Wed, 01 Nov 2023 01:47:49 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-01T01:38:36" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="e8510c65a9be4b0635372fd09bee126ce7e08bc7" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.3-1361"
# Wed, 01 Nov 2023 01:47:50 GMT
RUN rm -f '/etc/yum.repos.d/repo-7e938.repo' '/etc/yum.repos.d/repo-2aab0.repo'
# Wed, 01 Nov 2023 01:47:51 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 01 Nov 2023 01:47:52 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 08 Nov 2023 01:05:21 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 08 Nov 2023 01:05:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Nov 2023 01:05:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Nov 2023 01:05:27 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Wed, 08 Nov 2023 01:05:28 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 08 Nov 2023 01:05:44 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:05:45 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Wed, 08 Nov 2023 01:05:45 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:05:45 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:d0355d2288c7a677704d6bdc86642b802766b898fac18aadd39a3cbc2ad24d77`  
		Last Modified: Tue, 07 Nov 2023 12:07:48 GMT  
		Size: 36.0 MB (36032057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb135cb39ac72c9d295b180f03035a7ed93ee56542bdc5bb63fccc0aa079b76`  
		Last Modified: Wed, 08 Nov 2023 01:08:22 GMT  
		Size: 28.3 MB (28317034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12a675d356c38191586808d4b800fadda769443c0e444025c063d1e3f3810e7`  
		Last Modified: Wed, 08 Nov 2023 01:08:47 GMT  
		Size: 40.8 MB (40841387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8eb7fa175b7d31bf13d33c9d968605c496787c35ce18ad723dd6dbf3582d6d2`  
		Last Modified: Wed, 08 Nov 2023 01:07:49 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66242f4401daed9b44d1eb53d9089eb4bdb8517144d287b8260134417364d908`  
		Last Modified: Wed, 08 Nov 2023 01:08:43 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:92b3dc09e6c9a3838c7296fdbfcd6c94b4beb9f56bf35d10b8b8b93ac9263f00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113800507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c387559aab5de7c65b787a6ba268dd3234b4ab5d1b43e58ec01541b7b1f56117`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 01 Nov 2023 01:47:49 GMT
ADD file:9919b865596aaff36f0af850462ed61cc440218718ad76c59b0d42e841b000e8 in / 
# Wed, 01 Nov 2023 01:47:50 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 01 Nov 2023 01:47:51 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 01 Nov 2023 01:47:51 GMT
ADD multi:de99ba40d34adfc554e955bb344f3584a5587f990f2c5ac525d44349cf2c6f4b in /etc/yum.repos.d/ 
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.3"
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL io.openshift.expose-services=""
# Wed, 01 Nov 2023 01:47:51 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 01 Nov 2023 01:47:51 GMT
ENV container oci
# Wed, 01 Nov 2023 01:47:51 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 01:47:51 GMT
CMD ["/bin/bash"]
# Wed, 01 Nov 2023 01:47:52 GMT
RUN rm -rf /var/log/*
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL release=1361
# Wed, 01 Nov 2023 01:47:52 GMT
ADD file:c49d95a8d960474e9663d0df6aca76af53febdd007c6acbca0333c31b6f10da5 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.3-1361.json 
# Wed, 01 Nov 2023 01:47:52 GMT
ADD file:6ba5831b8aa27b1969a5b50db81939f011378fd76995d633d2bd8c55004db343 in /root/buildinfo/Dockerfile-ubi9-minimal-9.3-1361 
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-01T01:38:36" "architecture"="ppc64le" "vcs-type"="git" "vcs-ref"="e8510c65a9be4b0635372fd09bee126ce7e08bc7" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.3-1361"
# Wed, 01 Nov 2023 01:47:54 GMT
RUN rm -f '/etc/yum.repos.d/repo-7e938.repo' '/etc/yum.repos.d/repo-2aab0.repo'
# Wed, 01 Nov 2023 01:47:55 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 01 Nov 2023 01:47:56 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 08 Nov 2023 00:50:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 08 Nov 2023 00:50:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Nov 2023 00:50:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Nov 2023 00:50:54 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Wed, 08 Nov 2023 00:50:56 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 08 Nov 2023 00:51:30 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 00:51:32 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Wed, 08 Nov 2023 00:51:32 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 00:51:32 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:1ab516f84715e1e35f1c9b77be25d326cc2e44178f6afe6bdb92d199da9989fd`  
		Last Modified: Tue, 07 Nov 2023 12:07:55 GMT  
		Size: 42.1 MB (42146160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c4ed99d56ef3fc0e38058e8b626238825f1f9af17f2a8b895c2a60cf95cd75`  
		Last Modified: Wed, 08 Nov 2023 00:54:49 GMT  
		Size: 30.4 MB (30429407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f37cbd67f4428587fea8819f904942509b0ad84bcce7a38cde8857abf163ce`  
		Last Modified: Wed, 08 Nov 2023 00:55:14 GMT  
		Size: 41.2 MB (41224067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bed3e28d8cb5a5888fbbef6244bf9d19db1336fc409717a7408f561af70f85`  
		Last Modified: Wed, 08 Nov 2023 00:55:08 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3de838475fc478174e6202bcff102cb9415a9970e69f65b101541bc86b9cd19`  
		Last Modified: Wed, 08 Nov 2023 00:55:08 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
