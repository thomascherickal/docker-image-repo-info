## `eclipse-temurin:8-jdk-focal`

```console
$ docker pull eclipse-temurin@sha256:5142022ebe3437572f92c6003956612519ae92966fc251a218853eeacabfca3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:8-jdk-focal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:80a632fcdd8deea15f39147dce7bb626d42907041b6ab066068949fad7269d0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148109241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28f46d06509c51356ccc6acda8773002216fe1aa6751515960e291c2dca4ff4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:12:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:12:53 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Tue, 07 Jun 2022 00:13:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='d10efb2afad3ed3d7bac9d3249cea77928aca6acb973cac0f90a2dd3606a3533';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='c914250a736e620c12f9fe65fcd94ffa1acdacc5323e5aaff611a33a37cd158f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='1df8c12fd97e76c388d64e4df16893f4285e000e6ff837d1e39969e5428aafa0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='adc13a0a0540d77f0a3481b48f10d61eb203e5ad4914507d489c2de3bd3d83da';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 00:13:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 00:13:05 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caca7a4a00fe7d5efa72ecdbb346c7a4ee0e8e43c3a263d2bb79893d52bd4678`  
		Last Modified: Tue, 07 Jun 2022 00:19:21 GMT  
		Size: 16.0 MB (16029798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d20e7eb18a115970d8e31de2a9c872267288773da6497427d9599ed831514d`  
		Last Modified: Tue, 07 Jun 2022 00:19:27 GMT  
		Size: 103.5 MB (103506651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9defeaf1a778a43eb061f02eeadbcbcce20f07a55826c3018270b45f0a20a`  
		Last Modified: Tue, 07 Jun 2022 00:19:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk-focal` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:e0eb19f3954be4191c6f39af26b96e30abcf97205c71b46a1f81c12cd0b76be7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138666713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169c88b19e247b3258a95bfd0e5e2707530c87624942002d55041da04fa0f2f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:33:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 09:34:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:34:27 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Tue, 07 Jun 2022 09:34:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='d10efb2afad3ed3d7bac9d3249cea77928aca6acb973cac0f90a2dd3606a3533';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='c914250a736e620c12f9fe65fcd94ffa1acdacc5323e5aaff611a33a37cd158f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='1df8c12fd97e76c388d64e4df16893f4285e000e6ff837d1e39969e5428aafa0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='adc13a0a0540d77f0a3481b48f10d61eb203e5ad4914507d489c2de3bd3d83da';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:34:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:34:56 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ae1d24c2862f98f09de4a24a053161044e470b33c4e92d9f9807726bf4d12d`  
		Last Modified: Tue, 07 Jun 2022 09:51:03 GMT  
		Size: 14.9 MB (14902076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e5d7e2547b91a83a6bd684f13cb9162d9676999577ff76b1d59f91152d574a`  
		Last Modified: Tue, 07 Jun 2022 09:51:36 GMT  
		Size: 99.2 MB (99171838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce51f7e4a8d71dd1900439092e5b6a1ae5d97cd655ce96c33f82218300658627`  
		Last Modified: Tue, 07 Jun 2022 09:50:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk-focal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:966aa8e8529cd83c56e7a98b3d799aa6277065712682f6b471b67ede1c2dc0a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.7 MB (145685763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be91e08579ac5758317a0f0aa6d2219e29bed0979f9b0f89345dd153253ebe88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:59:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 05:00:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:34:18 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Tue, 07 Jun 2022 06:34:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='d10efb2afad3ed3d7bac9d3249cea77928aca6acb973cac0f90a2dd3606a3533';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='c914250a736e620c12f9fe65fcd94ffa1acdacc5323e5aaff611a33a37cd158f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='1df8c12fd97e76c388d64e4df16893f4285e000e6ff837d1e39969e5428aafa0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='adc13a0a0540d77f0a3481b48f10d61eb203e5ad4914507d489c2de3bd3d83da';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:34:26 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:34:27 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15da1b4c110f7cc460fbf968fb55b77c541f0e3ab87b92d5e6a822cc2c593e1`  
		Last Modified: Tue, 07 Jun 2022 05:10:23 GMT  
		Size: 15.9 MB (15898299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcece0580e10c416c1e7046a5470a31a642ce59eaf3a03ef9b31073f0fd3e91`  
		Last Modified: Tue, 07 Jun 2022 06:41:49 GMT  
		Size: 102.6 MB (102596127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c91f4a49be859828f6df357cf0f1808e1f6d00041b47ecc2e772bd926e536`  
		Last Modified: Tue, 07 Jun 2022 06:41:39 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk-focal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:3b3ec0512dd5bb64ac1c972c1219e6abd4de7a7f3ec7c91281f2de181c540b52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.5 MB (151502022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:468701847a2b79cb0edac22bf35d835c5fe2de575c16a1fe8a6b86968bc604cb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 07:18:17 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Tue, 07 Jun 2022 07:18:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='d10efb2afad3ed3d7bac9d3249cea77928aca6acb973cac0f90a2dd3606a3533';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='c914250a736e620c12f9fe65fcd94ffa1acdacc5323e5aaff611a33a37cd158f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='1df8c12fd97e76c388d64e4df16893f4285e000e6ff837d1e39969e5428aafa0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='adc13a0a0540d77f0a3481b48f10d61eb203e5ad4914507d489c2de3bd3d83da';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 07:18:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 07:18:46 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adeb595fe732411acad62cbc9426e0c74e8227209b52b3d2a5a951349c2c96d0`  
		Last Modified: Tue, 07 Jun 2022 07:30:25 GMT  
		Size: 101.0 MB (101003884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89c731f861e03b28d30382630e9cc1af7e8a8529035494bc617c07f6817b9e8`  
		Last Modified: Tue, 07 Jun 2022 07:30:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
