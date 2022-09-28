## `eclipse-temurin:19-jre-centos7`

```console
$ docker pull eclipse-temurin@sha256:5758c81d0e3cf3a584f4993f1209c82065c99da9f7989534c57839ffa13f1ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:19-jre-centos7` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:9954109e47a8a4aa6f271481ea952b0ac63da6a13363b5dda8bde2a0fb813caf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144191533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681fc9797e768c55d869517a5a94f016dbcd5ad3bd0a272b8c29c774f3e0845a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 11 Aug 2022 19:21:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:21:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:21:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:24:26 GMT
RUN yum install -y tzdata openssl curl wget ca-certificates fontconfig gzip tar binutils     && yum clean all
# Mon, 26 Sep 2022 23:22:05 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:23:40 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 28 Sep 2022 17:23:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e770a96dde57a5e5a0aa14457724aedca48015617007464fb8d5d08e84cedb`  
		Last Modified: Fri, 12 Aug 2022 17:33:04 GMT  
		Size: 18.8 MB (18784094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f20dc9d9ab629b71545e9139359c118f6cc4c9bc4375dcb40a2a12df44a3e7`  
		Last Modified: Wed, 28 Sep 2022 17:27:54 GMT  
		Size: 49.3 MB (49310123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347f4e8bf490d7eb21c37397f3aa3b4158aee88addda4e87c6ef06abf1a2f5a6`  
		Last Modified: Wed, 28 Sep 2022 17:27:47 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:19-jre-centos7` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:793a389f86446aa3c586452c478393744d1573f59b5df72c78a4de1c929eb250
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.5 MB (175467477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700b41034bc3ee2ede5f3bcb3b418b287645063af1482d7f49986f2cfb7a4421`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Thu, 11 Aug 2022 18:41:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:41:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:41:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:46:06 GMT
RUN yum install -y tzdata openssl curl wget ca-certificates fontconfig gzip tar binutils     && yum clean all
# Mon, 26 Sep 2022 22:42:02 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 16:44:52 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 28 Sep 2022 16:44:53 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7ff41d99b527a4020b8a26dbc2e07f3b75a5dc96a7f0adaf5ac46d3bafb569`  
		Last Modified: Fri, 12 Aug 2022 17:56:36 GMT  
		Size: 18.3 MB (18329548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59162a699416244b5a6c954e6f9573be3ce63d6ae63ca639900e4246ec8c5a`  
		Last Modified: Wed, 28 Sep 2022 16:50:13 GMT  
		Size: 48.8 MB (48762856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f649051b9efc1d43f096025d16bbfb2e4ecad35e34218a3c622075ef0d71e68`  
		Last Modified: Wed, 28 Sep 2022 16:50:06 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:19-jre-centos7` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:6f5e75e11be14cefbad4c555d57b0c6ed38221a27940a2612b4d7b4863066574
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148340638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:894be5892cc6915448d3e4f97f7858916a03fb4adeffe13265727b7e5e282d1d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:29:27 GMT
ADD file:7f21ae7d20a8e347d8b678bcf26be83abb1ee27d3b567c9cddd993e45ce8ac34 in / 
# Wed, 15 Sep 2021 18:29:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:29:40 GMT
CMD ["/bin/bash"]
# Thu, 11 Aug 2022 19:19:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:26:11 GMT
RUN yum install -y tzdata openssl curl wget ca-certificates fontconfig gzip tar binutils     && yum clean all
# Wed, 28 Sep 2022 17:19:20 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:20:32 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 28 Sep 2022 17:20:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:3fe478aaff9b8f3ba958253e7339e9016ec07c075b805ebfc8cd372ddd01ee64`  
		Last Modified: Tue, 17 Nov 2020 04:06:20 GMT  
		Size: 80.5 MB (80516460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401d76cfe8b1d20af213b24d4cc02ba53d59ecd1a910ea14d5c669b79827a6f0`  
		Last Modified: Fri, 12 Aug 2022 17:39:33 GMT  
		Size: 18.8 MB (18806203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c25f76ae1f95af285116eb5bf1c9d896d4ef534464734a54fe11b8ea3d36c3`  
		Last Modified: Wed, 28 Sep 2022 17:27:06 GMT  
		Size: 49.0 MB (49017815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee2c8b5eee38bff3d15de05fa2c242905bd99353e6caa4373115ab57f75b77a`  
		Last Modified: Wed, 28 Sep 2022 17:26:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
