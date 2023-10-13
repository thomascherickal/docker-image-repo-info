## `clojure:temurin-11-focal`

```console
$ docker pull clojure@sha256:29aa76c80438c7da02d343e5e530ff84278347594b5f020aa9e7d47d4dca2d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-focal` - linux; amd64

```console
$ docker pull clojure@sha256:f947b2647b51eddfc5c2f72f54506d3cc5b372e28415ed0ac9cd4364496ee444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.5 MB (253528522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65078e4781cd22acc7ef5a56fa5a28af629776b1d9ef90977cd15090954b5bf0`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:50:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:50:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:50:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 05:50:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:52:07 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 05:52:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 05:52:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 05:52:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 05:52:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 05:52:17 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 12:51:13 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 12:51:13 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:51:35 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 12:51:35 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 12:51:35 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ba2f5735c673e4fce5f702cdf0e513d89a91adfffc4e42977eae7cd354a0a`  
		Last Modified: Fri, 13 Oct 2023 05:56:23 GMT  
		Size: 16.9 MB (16919575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d677692c8a5373e6ee3b096be7076eae8d013ed651d83fc141c85527e81bb7`  
		Last Modified: Fri, 13 Oct 2023 05:57:46 GMT  
		Size: 144.8 MB (144837057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e66e5ce18ead7c0d7d222c41523a820292790767d90035db6be25ee830d3e3`  
		Last Modified: Fri, 13 Oct 2023 05:57:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18422839b9d0ec1b9e1569bf52d1f1530a90ffda19f071b6e03bbda620b267`  
		Last Modified: Fri, 13 Oct 2023 05:57:34 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44952263d6a456369baeb8c0de9a44cb1d42519ddf5f904ac5d76d32704d4a83`  
		Last Modified: Fri, 13 Oct 2023 13:09:07 GMT  
		Size: 63.2 MB (63189675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28739fb2cc50a61d1cb85d39d46c6993098c14a79e975de765728d11fbebbb9`  
		Last Modified: Fri, 13 Oct 2023 13:08:59 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1551d9fac9898de0c6b83274f6511d1a354fc4fe223b99f4a452cb3c3865f62d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248885468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca08606552d35e35669c32f45820c7b3c388b0859e46bfb0bd26c3cc87397e62`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 02:46:20 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:47:16 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 02:47:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 02:47:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 02:47:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 02:47:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 02:47:28 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 10:18:06 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 10:18:06 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:18:19 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 10:18:20 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 10:18:20 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7fe5b0236efc346cd4debc4c5e5b3c24c2c34ab5913c1647b26219f2c53f7`  
		Last Modified: Fri, 13 Oct 2023 02:50:41 GMT  
		Size: 16.8 MB (16768291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84562ffe350fd123902a28225215826843d7983e543835f54b2af29c6e3ce992`  
		Last Modified: Fri, 13 Oct 2023 02:51:51 GMT  
		Size: 141.6 MB (141584461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bd8ecdd6a33dcccec3d07709e6f8f48487b45cfb79709d88776ac6325faf6a`  
		Last Modified: Fri, 13 Oct 2023 02:51:42 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b93572998af73b5ca61b23f8a00ca5bf4b6fdbf25853fbc3a76cdff635f9ff`  
		Last Modified: Fri, 13 Oct 2023 02:51:42 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5620f34f16b87dc568c3942fb56742db2c545a489f94426e6af34ae290943ef3`  
		Last Modified: Fri, 13 Oct 2023 10:33:23 GMT  
		Size: 63.3 MB (63331677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba21a3472570c5f7655a0b1c9d7100dfed7af3c58684e9267100c8c40804ee90`  
		Last Modified: Fri, 13 Oct 2023 10:33:16 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
