## `maven:3-eclipse-temurin-17-focal`

```console
$ docker pull maven@sha256:624773bbf944c7d53cde3a92884f659f4d8ff03b1d1ef3c41e7e85830846a423
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-eclipse-temurin-17-focal` - linux; amd64

```console
$ docker pull maven@sha256:2510cc98c9eac0a8839f92fddd08826d272a892be0acee3f34640847cc27fa1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280421151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865a673b5cafec8f28e3218c8298b7d12f02b9a3f95c15d2aeed1f7e0dc6fcfa`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:15:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 16:22:08 GMT
ENV JAVA_VERSION=jdk-17.0.4+8
# Thu, 28 Jul 2022 16:22:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c23b0b9c65cfe223a07edb8752026afd1e8ec1682630c2d92db4dd5aa039204';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4_8.tar.gz';          ;;        armhf|arm)          ESUM='f499656e581517e62aa954965a7a19bbb0ea8c2e6bd84050527b88efbaa1d96d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='e80a0f6626bd28ea20c43524b3ab10af48b3789317aea5b7019c146fe6268d94';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='40b09e8fa473f194030a85c059ba768abf5635a9a6d4dbeb79a87113ee8f4ece';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c0851d610b03cb51e9b360fef3e9ec2026c62837a143e7786649ba94f38cc0d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Jul 2022 16:22:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 16:22:17 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 28 Jul 2022 16:22:18 GMT
CMD ["jshell"]
# Thu, 28 Jul 2022 19:00:13 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 19:00:14 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 28 Jul 2022 19:00:14 GMT
ARG USER_HOME_DIR=/root
# Thu, 28 Jul 2022 19:00:14 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 28 Jul 2022 19:00:14 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 28 Jul 2022 19:00:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 28 Jul 2022 19:00:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 28 Jul 2022 19:00:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 28 Jul 2022 19:00:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 28 Jul 2022 19:00:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 28 Jul 2022 19:00:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 28 Jul 2022 19:00:16 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32598539a8f0b55be77078c6637866fc4128a4213ea59e9993662a310a2b711`  
		Last Modified: Tue, 07 Jun 2022 00:22:05 GMT  
		Size: 19.8 MB (19773881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33710839ca3af3d6a583c0b8b9091270cf89851f5c03fc9d15f43645e5745551`  
		Last Modified: Thu, 28 Jul 2022 16:28:52 GMT  
		Size: 192.1 MB (192148048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63208a3f8de08e4ec3b0e482f7b081a286a8a9f77ab1193c240a27a76e1df5cb`  
		Last Modified: Thu, 28 Jul 2022 16:28:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a68a30795189fd1720bf0703746b0b8a65efd209f2f9fc8805206e5f10ff79`  
		Last Modified: Thu, 28 Jul 2022 19:04:18 GMT  
		Size: 31.2 MB (31185739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc2844e02b226a73343dda931bbe535031c059a21e873eb6a26a7c600c2a1d3`  
		Last Modified: Thu, 28 Jul 2022 19:04:14 GMT  
		Size: 8.7 MB (8739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d105d2264ef1798e7655dcc3b0812a0a4740eda0deb93626349050baed8ed9`  
		Last Modified: Thu, 28 Jul 2022 19:04:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208256c36225bc15d25dc7bb5bb2eead4adac8a43dbc87a23d6b49fbdf916144`  
		Last Modified: Thu, 28 Jul 2022 19:04:13 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-17-focal` - linux; arm variant v7

```console
$ docker pull maven@sha256:72200711262d020ba88a5101727b96a0149c2459b3cd3efda7886cca2561b072
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268898767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823d82af764acab4fb2d4e781cf72be3dd1760272f755d8f5b7202ebf204db8f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Sat, 30 Jul 2022 02:49:11 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Jul 2022 02:52:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Jul 2022 02:52:16 GMT
ENV JAVA_VERSION=jdk-17.0.4+8
# Sat, 30 Jul 2022 02:52:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c23b0b9c65cfe223a07edb8752026afd1e8ec1682630c2d92db4dd5aa039204';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4_8.tar.gz';          ;;        armhf|arm)          ESUM='f499656e581517e62aa954965a7a19bbb0ea8c2e6bd84050527b88efbaa1d96d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='e80a0f6626bd28ea20c43524b3ab10af48b3789317aea5b7019c146fe6268d94';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='40b09e8fa473f194030a85c059ba768abf5635a9a6d4dbeb79a87113ee8f4ece';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c0851d610b03cb51e9b360fef3e9ec2026c62837a143e7786649ba94f38cc0d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Jul 2022 02:52:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Jul 2022 02:52:35 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 30 Jul 2022 02:52:35 GMT
CMD ["jshell"]
# Sat, 30 Jul 2022 12:44:04 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Jul 2022 12:44:04 GMT
ARG MAVEN_VERSION=3.8.6
# Sat, 30 Jul 2022 12:44:04 GMT
ARG USER_HOME_DIR=/root
# Sat, 30 Jul 2022 12:44:04 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Sat, 30 Jul 2022 12:44:04 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Sat, 30 Jul 2022 12:44:06 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 30 Jul 2022 12:44:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 30 Jul 2022 12:44:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 30 Jul 2022 12:44:06 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 30 Jul 2022 12:44:07 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 30 Jul 2022 12:44:07 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 30 Jul 2022 12:44:07 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916985a90d5d9c5f2a2e834acb83d3a31a527d90f6140d699201612fc01376a1`  
		Last Modified: Sat, 30 Jul 2022 02:59:50 GMT  
		Size: 19.2 MB (19191327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7002f75bff32937ce0528d7d2f3441be5099ab9813fcd444d847b3eb45a469`  
		Last Modified: Sat, 30 Jul 2022 03:00:04 GMT  
		Size: 189.1 MB (189067034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c378c698697a5286247ca246ea46e785821f7131163eeddcf0fa51a1cc9fc8`  
		Last Modified: Sat, 30 Jul 2022 02:59:46 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609646a50af89c7645c4129e9eef24706e98e6bc25c698c39ae5e1b513f0c229`  
		Last Modified: Sat, 30 Jul 2022 12:48:18 GMT  
		Size: 27.3 MB (27306907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1017dd0f9e8c75e4c782e41c2c4b9c6f7b1fc60178204580e0e6dd5718f9be`  
		Last Modified: Sat, 30 Jul 2022 12:48:15 GMT  
		Size: 8.7 MB (8739487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe5062d8cb754e2d10f4e015a63b6f77103848a919937e5d8e3f4afae289320`  
		Last Modified: Sat, 30 Jul 2022 12:48:14 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a90aa06b74528d7ded23fd858f733fdd9640e2f86aa20c51f11e7a22274cc`  
		Last Modified: Sat, 30 Jul 2022 12:48:14 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-17-focal` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ab8871f3990f369b8bc2f1d4d81d798b3c9cb5d4de142b3a9461bef5731f299f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278317970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16a41baa412aa3933712b25215bb6ac9a2018d932e94debea46af3d6f44c532`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:50:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 17:54:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:54:11 GMT
ENV JAVA_VERSION=jdk-17.0.4+8
# Tue, 02 Aug 2022 17:54:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c23b0b9c65cfe223a07edb8752026afd1e8ec1682630c2d92db4dd5aa039204';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4_8.tar.gz';          ;;        armhf|arm)          ESUM='f499656e581517e62aa954965a7a19bbb0ea8c2e6bd84050527b88efbaa1d96d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='e80a0f6626bd28ea20c43524b3ab10af48b3789317aea5b7019c146fe6268d94';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='40b09e8fa473f194030a85c059ba768abf5635a9a6d4dbeb79a87113ee8f4ece';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c0851d610b03cb51e9b360fef3e9ec2026c62837a143e7786649ba94f38cc0d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 17:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 17:54:21 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 02 Aug 2022 17:54:22 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 01:05:51 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:05:52 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 01:05:52 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 01:05:53 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 01:05:54 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 01:05:57 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 01:05:58 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 01:05:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 01:06:01 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 01:06:02 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 01:06:02 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 01:06:03 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae4b399269fa184aac3bbe66763d5b373c71d601c49266b8828e09b7fdd6789`  
		Last Modified: Tue, 02 Aug 2022 18:03:22 GMT  
		Size: 20.5 MB (20491864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b6fa7266c6e5b9c9edc2ca6a44b58e9b744191d14d57c7e49ef9d9c309fcc8`  
		Last Modified: Tue, 02 Aug 2022 18:03:40 GMT  
		Size: 190.9 MB (190907080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e36ccee0fb296aaf6b1dc8c8b2e78fb031f1e75b36c69818820a3abc86dc2e2`  
		Last Modified: Tue, 02 Aug 2022 18:03:19 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8515199aed690f17fd459d286558f139079e125af947d32de970afcf67fa9e`  
		Last Modified: Wed, 03 Aug 2022 01:15:39 GMT  
		Size: 31.0 MB (30986404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70697395b3587fd817f139b25add6b5ce285188aeb6cbfeb8b18703c2e61ecf`  
		Last Modified: Wed, 03 Aug 2022 01:15:35 GMT  
		Size: 8.7 MB (8739477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ccc32a8dab868b98c6f128c2a1d5fe3222dbd0713edb554ca3623f7e181f5`  
		Last Modified: Wed, 03 Aug 2022 01:15:34 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329c8e396093a700c4dc9ffe3ade03b8d9331b0788f194fdee474f204079a442`  
		Last Modified: Wed, 03 Aug 2022 01:15:34 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-17-focal` - linux; ppc64le

```console
$ docker pull maven@sha256:4d65b21fc1b017d751fb9ad80174bcceb3e5169d5902d220f3041410b8431615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.6 MB (293567494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1ffcbec0e2ee9bb4717797d6417f22067514f974825ec5dc81273f437d4d46`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Wed, 27 Jul 2022 00:33:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 27 Jul 2022 00:41:17 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 16:19:37 GMT
ENV JAVA_VERSION=jdk-17.0.4+8
# Thu, 28 Jul 2022 16:19:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c23b0b9c65cfe223a07edb8752026afd1e8ec1682630c2d92db4dd5aa039204';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4_8.tar.gz';          ;;        armhf|arm)          ESUM='f499656e581517e62aa954965a7a19bbb0ea8c2e6bd84050527b88efbaa1d96d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='e80a0f6626bd28ea20c43524b3ab10af48b3789317aea5b7019c146fe6268d94';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='40b09e8fa473f194030a85c059ba768abf5635a9a6d4dbeb79a87113ee8f4ece';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c0851d610b03cb51e9b360fef3e9ec2026c62837a143e7786649ba94f38cc0d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Jul 2022 16:20:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 16:20:03 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 28 Jul 2022 16:20:03 GMT
CMD ["jshell"]
# Thu, 28 Jul 2022 18:12:22 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 18:12:23 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 28 Jul 2022 18:12:23 GMT
ARG USER_HOME_DIR=/root
# Thu, 28 Jul 2022 18:12:24 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 28 Jul 2022 18:12:24 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 28 Jul 2022 18:12:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 28 Jul 2022 18:12:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 28 Jul 2022 18:12:26 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 28 Jul 2022 18:12:27 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 28 Jul 2022 18:12:27 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 28 Jul 2022 18:12:27 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 28 Jul 2022 18:12:27 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff6ca525e26e65e4f33725ff2f731fb66f9fa21452fe1cff1f1d65d9860921`  
		Last Modified: Wed, 27 Jul 2022 00:55:32 GMT  
		Size: 21.7 MB (21686416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17daab17b2aef799b4951369e50d9c0a7cceb99373271e2976c509578d769093`  
		Last Modified: Thu, 28 Jul 2022 16:28:36 GMT  
		Size: 191.5 MB (191454045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6a1e3205f38686d1e880f9060bd2e2c0b7f2a38a5c661a7325d2fb3b7d9e0`  
		Last Modified: Thu, 28 Jul 2022 16:28:11 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31790cae746e6741047ece49161f66b4ab080de66a08872fb74e7a02959e801`  
		Last Modified: Thu, 28 Jul 2022 18:16:29 GMT  
		Size: 38.4 MB (38391828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d47c77a98c1395a99e0f1fd6d6ff9cf9fcf48ac7d506f50accf6036dab5bec`  
		Last Modified: Thu, 28 Jul 2022 18:16:20 GMT  
		Size: 8.7 MB (8739485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927752abbc67da883039c8fea89faf56dcc9b86b35e1d32d21ac9b99654c8d99`  
		Last Modified: Thu, 28 Jul 2022 18:16:19 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f696b71f576dae71e5359c44df4e520875f33fafaf7cae06943d91a895fb72`  
		Last Modified: Thu, 28 Jul 2022 18:16:19 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-17-focal` - linux; s390x

```console
$ docker pull maven@sha256:3f805808ed2faf41e9b0ab77eb5dfc426cb9fcde5c2f62de54d4c03f19ce05ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.9 MB (265868930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57364f819775a296e4c39c52d4d7c9f62290be85d33574aee22d5b6baeca8ff`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:49:17 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:04:47 GMT
ENV JAVA_VERSION=jdk-17.0.4+8
# Tue, 02 Aug 2022 13:04:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c23b0b9c65cfe223a07edb8752026afd1e8ec1682630c2d92db4dd5aa039204';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4_8.tar.gz';          ;;        armhf|arm)          ESUM='f499656e581517e62aa954965a7a19bbb0ea8c2e6bd84050527b88efbaa1d96d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='e80a0f6626bd28ea20c43524b3ab10af48b3789317aea5b7019c146fe6268d94';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='40b09e8fa473f194030a85c059ba768abf5635a9a6d4dbeb79a87113ee8f4ece';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c0851d610b03cb51e9b360fef3e9ec2026c62837a143e7786649ba94f38cc0d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 13:05:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 13:05:07 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 02 Aug 2022 13:05:07 GMT
CMD ["jshell"]
# Tue, 02 Aug 2022 23:59:25 GMT
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 23:59:29 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 02 Aug 2022 23:59:30 GMT
ARG USER_HOME_DIR=/root
# Tue, 02 Aug 2022 23:59:30 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 02 Aug 2022 23:59:31 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 02 Aug 2022 23:59:35 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 02 Aug 2022 23:59:36 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 02 Aug 2022 23:59:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 02 Aug 2022 23:59:37 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 02 Aug 2022 23:59:38 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 02 Aug 2022 23:59:38 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 02 Aug 2022 23:59:39 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b48d17296789cbed49100fd665aec2330de5c27d57190835247afb1fa0799b`  
		Last Modified: Tue, 02 Aug 2022 12:54:34 GMT  
		Size: 19.2 MB (19224154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd470baa3b995832fd172ae46ac73c84b13fe4e6ef4d8fd89eb4321c90cf71d8`  
		Last Modified: Tue, 02 Aug 2022 13:10:22 GMT  
		Size: 180.2 MB (180161334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b526172fd5928f862f75fc9b2aaace9162d12a09d937dffc5a8fa566589fd589`  
		Last Modified: Tue, 02 Aug 2022 13:10:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e67ddf30f49fd64db34a20f9fd3f41f93ef41ec4630b65765b588cb92544464`  
		Last Modified: Wed, 03 Aug 2022 00:06:42 GMT  
		Size: 30.7 MB (30697217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10c4d90afc960712af23d0884754b0212214d44587e7e4e2e2319f254ad8b9b`  
		Last Modified: Wed, 03 Aug 2022 00:06:38 GMT  
		Size: 8.7 MB (8739488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199299186984d7bbd98711fbb331b054770a8601d75a3032cf491ee8556f3f5`  
		Last Modified: Wed, 03 Aug 2022 00:06:37 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef53b109933212a9fa48d17283b450ed053e3b25914493623ddbf39a0a17bb41`  
		Last Modified: Wed, 03 Aug 2022 00:06:38 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
