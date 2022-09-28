## `eclipse-temurin:19-jre-focal`

```console
$ docker pull eclipse-temurin@sha256:0ebc21c91ae3d9e75a2f9b6b1c17f5471cb16832e6c07e34b17822dd47ea6671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:19-jre-focal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:f56af9c7a7b2557d733a7d6b5c494fb0e5329a96d5ac70f40724981ac3b855f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97994040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116c072b11c111795efd7bdf486c89b82409dd0ea971fb9769a324e7e13df4f2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:21:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 05:21:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 05:21:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 05:24:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Sep 2022 23:21:02 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:23:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        armhf|arm)          ESUM='f6c4895b8d33118c75403d08f9697af0b77769d0e8574cb678518a0ab3b74a12';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_arm_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 28 Sep 2022 17:23:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b5511391049b7fe5160b78ebae36e40eef43734a07d246dc389dff107a1d22`  
		Last Modified: Fri, 02 Sep 2022 05:30:57 GMT  
		Size: 20.1 MB (20104278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed07fc42c99543990af3a8ee775563dd400ecff2af89c1f06819ceeebdc45c4`  
		Last Modified: Wed, 28 Sep 2022 17:27:20 GMT  
		Size: 49.3 MB (49316918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709e0ce2e0c7a3b5d7a6ecbca69e651f91314144ffe62e16b6da8f04902908df`  
		Last Modified: Wed, 28 Sep 2022 17:27:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:19-jre-focal` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:ea0911807dc2afe9026dc2c9864a73240b0cae70319a711c4a337514c9fee966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90395549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dce2736271cb54053f43040fddec4192765644dc7eead0d484ee331d47420cf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:44:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:44:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 09:48:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Sep 2022 10:02:36 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:51:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        armhf|arm)          ESUM='f6c4895b8d33118c75403d08f9697af0b77769d0e8574cb678518a0ab3b74a12';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_arm_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 28 Sep 2022 17:51:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d190108b6a94c1cc5797e9f9665782f822a4af6e6a760fcb7014d05f1ee0759`  
		Last Modified: Fri, 02 Sep 2022 09:55:47 GMT  
		Size: 19.5 MB (19486989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d24f07aa65019203a54dca9e3b0b695a55b188926ab57b920abc60627819ef`  
		Last Modified: Wed, 28 Sep 2022 17:55:17 GMT  
		Size: 46.3 MB (46319658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3055cde9fe4f6495fbe6a932fc30df895cad66c9abe3e1d354fcff70d80acc5c`  
		Last Modified: Wed, 28 Sep 2022 17:55:09 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:19-jre-focal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:540f4844771df81c73502475af048411492b9baf23e8726e01a2b0088c61a9bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96781465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950e373574e72b75d7afc31e5ba0359525b6b4d222e5987c80a470076cb7ec3c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:55:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 04:55:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 04:55:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 04:58:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Sep 2022 22:41:15 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 16:44:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        armhf|arm)          ESUM='f6c4895b8d33118c75403d08f9697af0b77769d0e8574cb678518a0ab3b74a12';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_arm_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 28 Sep 2022 16:44:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acfbc542a09b96c46a1e01db8b85890c47a99e4b81a47aaaefb32912107321d`  
		Last Modified: Fri, 02 Sep 2022 05:07:16 GMT  
		Size: 20.8 MB (20824963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d85b481523f94f7ef49dc65e4c424fd6cef0782e93194bd6b29ffdb9b22e74`  
		Last Modified: Wed, 28 Sep 2022 16:49:33 GMT  
		Size: 48.8 MB (48764528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a093e99f6adcb4366c2f7d4732a440f5f976613df95be47e0f632c4386f6b46`  
		Last Modified: Wed, 28 Sep 2022 16:49:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:19-jre-focal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:1d538f97f90e92afb3fef82bebecdcaf250806bff0dc6b10a8647d2687fcb855
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104396136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0256193721f4bc4ef030a355643c4cb3abaf25f99ea176717e854188ab261b2e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 04:00:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 04:00:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 04:05:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Sep 2022 17:18:11 GMT
ENV JAVA_VERSION=jdk-19+36
# Wed, 28 Sep 2022 17:20:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='da77060192d3021a2e06eb51a91acdfacb0b993fc75a3b4cafe9c39c6132cc51';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_aarch64_linux_hotspot_19_36.tar.gz';          ;;        armhf|arm)          ESUM='f6c4895b8d33118c75403d08f9697af0b77769d0e8574cb678518a0ab3b74a12';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_arm_linux_hotspot_19_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3ab0b2320d5bb0f2fef9fd831338fd51170e6b8db887af23bc26dfc51bdf338c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_ppc64le_linux_hotspot_19_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ef2caf3221cb3d209ba7662d9542f23e25b3b97696de3103264c5a519aad30b6';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jre_x64_linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 28 Sep 2022 17:20:02 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be295fe80776586a1665f42f6aa8a3d7eb91486194e2537a9c4651eefea0b183`  
		Last Modified: Fri, 02 Sep 2022 04:16:22 GMT  
		Size: 22.1 MB (22078715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a63d2ad5cbcf70a896d1002d185b96789c7c80bac9cac2e8c3db07d2117d7ba`  
		Last Modified: Wed, 28 Sep 2022 17:26:18 GMT  
		Size: 49.0 MB (49021637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34f3541e7215416869368dee702520b7f98441cd21631ac4b1b8bc27384a92d`  
		Last Modified: Wed, 28 Sep 2022 17:26:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
