## `eclipse-temurin:8-ubi9-minimal`

```console
$ docker pull eclipse-temurin@sha256:a21045efe4bdba32883b89cdd6d0b5d7048cecf151d692e52f9366eb9deeaa77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:8-ubi9-minimal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:3c1ff5bb344ca058b1aff869191b20d2ff0fb1bb89d2c9bcec949ba5b048322d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169210943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205eff3b74144a6d7c22a48d04b9905903ef001070f15e04da25afc53c5f58ae`
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
# Wed, 08 Nov 2023 01:10:51 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:10:52 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Wed, 08 Nov 2023 01:10:52 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:10:52 GMT
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
	-	`sha256:8246582237e977247394efeab17ff724c88fda084e02e7863c7e9385cff1c484`  
		Last Modified: Wed, 08 Nov 2023 01:14:30 GMT  
		Size: 103.6 MB (103598542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc743d8a68e095193298e65f4853f889e0bd3dc8d50ebd2fdca02e497dc129d`  
		Last Modified: Wed, 08 Nov 2023 01:14:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09aefbcead9db0b73d7a0dafc834217c687294c0ddbd43abd963fd9c072d721`  
		Last Modified: Wed, 08 Nov 2023 01:14:21 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-ubi9-minimal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:0254fcacd548f32937eb8cc5fdd02e32116e62bbd320c74b4c663d00493d6ee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.1 MB (167051793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5e877e28f4a8e21ebd33e2a9ccec1696fa3c37744e0c495301bb91ae1cacd3`
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
# Wed, 08 Nov 2023 01:05:32 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 01:05:34 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Wed, 08 Nov 2023 01:05:34 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 01:05:34 GMT
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
	-	`sha256:f37426ceb3da6280274b8cdd8563e30b1a3b73543be4615a1b8c1783b5fedf4c`  
		Last Modified: Wed, 08 Nov 2023 01:08:28 GMT  
		Size: 102.7 MB (102701830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c8dde698958bc30830d4f8b70e8a2f1dc5c5b31a2b028e2385dda42b88410b`  
		Last Modified: Wed, 08 Nov 2023 01:08:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f2ce148b6b920468d1ef8a65ae2c6a72ec52b8689f43d2c3951b467d66f35e`  
		Last Modified: Wed, 08 Nov 2023 01:08:19 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-ubi9-minimal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:9c7518a8b726d603815752f65fb42170981efa5b60c8cf846322ec357fed3d70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173641019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d70f7c69f8e263d3a51440a125ac9cff980b299c1968942118c77d2ad6abf`
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
# Wed, 08 Nov 2023 00:51:05 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 08 Nov 2023 00:51:09 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Wed, 08 Nov 2023 00:51:10 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Wed, 08 Nov 2023 00:51:10 GMT
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
	-	`sha256:8d20a637f05e753c749543aef7d6c3f08c426a63ad42e945b9425d020655d70a`  
		Last Modified: Wed, 08 Nov 2023 00:54:53 GMT  
		Size: 101.1 MB (101064582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80558815bfaed7d828ecbc94e4247d0af1edaeb1e85a5caa65ead904ee57ce5`  
		Last Modified: Wed, 08 Nov 2023 00:54:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8708971a956592a5a79d09fd98d710f367b669f5cdcb94125963bf2407916410`  
		Last Modified: Wed, 08 Nov 2023 00:54:44 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
