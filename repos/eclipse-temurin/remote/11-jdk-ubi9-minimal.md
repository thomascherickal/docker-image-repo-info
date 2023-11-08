## `eclipse-temurin:11-jdk-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:cf969ab8fb7a704f4ede42dd22dff6877828ef7dd4ebc287e27882ea14361b79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:11-jdk-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:1f97668b9de50f91766c5bc69970f387f5724095b6a366181462d156400f3c42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.3 MB (207343672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546aaec675da00c7838d54d3664b89001ba0607ceaef629611debaac17df066d`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

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
# Wed, 08 Nov 2023 01:11:21 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 08 Nov 2023 01:11:29 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:11:32 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Wed, 08 Nov 2023 01:11:32 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:11:32 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 08 Nov 2023 01:11:32 GMT
CMD ["jshell"]
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
	-	`sha256:f1f13704bc77ab67ef45b527ed8ad0a86917144745b508ee8b2f7442d3ccab48`  
		Last Modified: Wed, 08 Nov 2023 01:15:21 GMT  
		Size: 141.7 MB (141731257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e65ef4f660cf57f5b48e9186a57a170b68f3ade5febbcddf7bfb8704abbc60`  
		Last Modified: Wed, 08 Nov 2023 01:15:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c38486d5aeda206005b450bc27ede98d68c3b007df79a81345aae4b48e52412`  
		Last Modified: Wed, 08 Nov 2023 01:15:07 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:d2b9bcee33356e128db11e4e2a0ddfbd66f29e3ebc1e3eb22578cea7110d0664
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202817307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f791705ac26ddc414af72c5a59239d9ae1d9e369b4c2b98009f657e02d1c686e`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

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
# Wed, 08 Nov 2023 01:05:52 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 08 Nov 2023 01:06:00 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:06:03 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Wed, 08 Nov 2023 01:06:04 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:06:04 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 08 Nov 2023 01:06:04 GMT
CMD ["jshell"]
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
	-	`sha256:5a6912d41c2c621e077fdb042d205ddbdd295519371f0a76a6bcdbbd039b7dad`  
		Last Modified: Wed, 08 Nov 2023 01:09:09 GMT  
		Size: 138.5 MB (138467328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3f381ddc9b845732fe0861a3bceff11f321811c8db903df90cd3e0072fd7df`  
		Last Modified: Wed, 08 Nov 2023 01:09:00 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9d449f6e2aa41d86197d18b2071baa4d5a0ff3879c618ee077863cf6d5b60`  
		Last Modified: Wed, 08 Nov 2023 01:09:00 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:d2eeeaa6f6735140ea9c1cde25eb5dc50925715a1db2a0b59fd16f89d97a1f26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201479797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde4fdfe0b378e6059709f6e2520847d73cee2779a9acc26ba7c3265f0f805fa`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

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
# Wed, 08 Nov 2023 00:51:42 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 08 Nov 2023 00:51:53 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 00:51:59 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Wed, 08 Nov 2023 00:51:59 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 00:52:00 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 08 Nov 2023 00:52:00 GMT
CMD ["jshell"]
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
	-	`sha256:3d4e2d51c5f806ac2452125f24597848d2d56ac9ad7402d8602593952784aa0b`  
		Last Modified: Wed, 08 Nov 2023 00:55:37 GMT  
		Size: 128.9 MB (128903343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b55752277691ff29363b1b80656f68f54310db51dabd3d4904a40d08e55339`  
		Last Modified: Wed, 08 Nov 2023 00:55:26 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c135cea69bc7ff1a5c3265ad8def741f58b5b53a718ee8beddf38a2e7426ba0a`  
		Last Modified: Wed, 08 Nov 2023 00:55:26 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-ubi9-minimal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:91467326f5e290a61ff3692afcb6238cbc7d674b36dff0a312c4aa4d1f0fd231
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.7 MB (185707678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceff50a372ca53e4a5c0b82812117efd2136e7309840ce0643360fe9dc376f12`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 01 Nov 2023 01:47:51 GMT
ADD file:7444bdc969a3b7d70c67575deb0e7022a94a71c46be753bd690def3d82a29f2f in / 
# Wed, 01 Nov 2023 01:47:52 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 01 Nov 2023 01:47:52 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 01 Nov 2023 01:47:52 GMT
ADD multi:de99ba40d34adfc554e955bb344f3584a5587f990f2c5ac525d44349cf2c6f4b in /etc/yum.repos.d/ 
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL com.redhat.component="ubi9-minimal-container"       name="ubi9-minimal"       version="9.3"
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 9."
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 9 Minimal"
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL io.openshift.expose-services=""
# Wed, 01 Nov 2023 01:47:52 GMT
LABEL io.openshift.tags="minimal rhel9"
# Wed, 01 Nov 2023 01:47:52 GMT
ENV container oci
# Wed, 01 Nov 2023 01:47:52 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 01:47:52 GMT
CMD ["/bin/bash"]
# Wed, 01 Nov 2023 01:47:53 GMT
RUN rm -rf /var/log/*
# Wed, 01 Nov 2023 01:47:53 GMT
LABEL release=1361
# Wed, 01 Nov 2023 01:47:54 GMT
ADD file:fe0700b8811b6303890f1c508217b622588787bab0672a58a4be7cdc3c0a2da5 in /root/buildinfo/content_manifests/ubi9-minimal-container-9.3-1361.json 
# Wed, 01 Nov 2023 01:47:54 GMT
ADD file:a46a8ee41e022b94f943713901ef5999011c67aa8df724c730f8eacb9320fc1b in /root/buildinfo/Dockerfile-ubi9-minimal-9.3-1361 
# Wed, 01 Nov 2023 01:47:54 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-01T01:38:36" "architecture"="s390x" "vcs-type"="git" "vcs-ref"="e8510c65a9be4b0635372fd09bee126ce7e08bc7" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi9-minimal/images/9.3-1361"
# Wed, 01 Nov 2023 01:47:55 GMT
RUN rm -f '/etc/yum.repos.d/repo-7e938.repo' '/etc/yum.repos.d/repo-2aab0.repo'
# Wed, 01 Nov 2023 01:47:56 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 01 Nov 2023 01:47:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Wed, 08 Nov 2023 01:04:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 08 Nov 2023 01:04:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Nov 2023 01:04:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Nov 2023 01:05:05 GMT
RUN set -eux;     microdnf install -y         gzip         tar         binutils         tzdata         openssl         wget         ca-certificates         fontconfig         glibc-langpack-en     ;     microdnf clean all
# Wed, 08 Nov 2023 01:05:06 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 08 Nov 2023 01:05:13 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:05:18 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Wed, 08 Nov 2023 01:05:18 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:05:18 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 08 Nov 2023 01:05:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d1b1e8ca5e96983a272ffb8698086457420cf1d591d2a93fd73f1237fed30a26`  
		Last Modified: Tue, 07 Nov 2023 12:08:00 GMT  
		Size: 36.0 MB (35974120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0706fb2c6305dfde885f31fdf5e771e9d3dd6006aa05c178accf0af44ff2b9`  
		Last Modified: Wed, 08 Nov 2023 01:07:35 GMT  
		Size: 27.9 MB (27925955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3140579139217c1144ed113d45ebaea404eb97258e04c8b8eb179dae5df3df0`  
		Last Modified: Wed, 08 Nov 2023 01:07:40 GMT  
		Size: 121.8 MB (121806716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9c1897118ddc5116ed543962f72dd1fe77ce4934ee7cccf6cc277c524971c9`  
		Last Modified: Wed, 08 Nov 2023 01:07:31 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca39d0e39936953bfa2252add197e2192b434b757afbd5360c4e10bc3a78092b`  
		Last Modified: Wed, 08 Nov 2023 01:07:32 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
