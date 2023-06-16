## `clojure:temurin-8-boot`

```console
$ docker pull clojure@sha256:8adbb2d98c4eec55c7a4fc6e4c93ff24ef8b56b4a1c8baf9120917ad05e236ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot` - linux; amd64

```console
$ docker pull clojure@sha256:faf2bc16f679fa4d2e1542e9d3d440dcf68853d6a0c410becbde31cc3776f30e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.7 MB (156727830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4a1509809eff03dde1c30fc86b04b0e78829c1343ae850ede30aa6c1010889b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:42:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Jun 2023 01:42:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 01:42:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Jun 2023 01:43:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:43:03 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Fri, 02 Jun 2023 01:43:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='195808eb42ab73535c84de05188914a52a47c1ac784e4bf66de95fe1fd315a5a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        armhf|arm)          ESUM='3f4848700a4bf856d3c138dc9c2b305b978879c8fbef5aa7df34a7c2fe1b64b8';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u372b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='bb85303848fe402d4f1004f748f80ccb39cb11f356f50a513555d1083c3913b8';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='78a0b3547d6f3d46227f2ad8c774248425f20f1cd63f399b713f0cdde2cc376c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 02 Jun 2023 01:43:09 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Sun, 04 Jun 2023 15:52:03 GMT
ENV BOOT_VERSION=2.8.3
# Sun, 04 Jun 2023 15:52:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sun, 04 Jun 2023 15:52:03 GMT
WORKDIR /tmp
# Sun, 04 Jun 2023 15:52:07 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sun, 04 Jun 2023 15:52:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 04 Jun 2023 15:52:07 GMT
ENV BOOT_AS_ROOT=yes
# Sun, 04 Jun 2023 15:52:34 GMT
RUN boot
# Sun, 04 Jun 2023 15:52:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7723b4ddeaefdff460e5e80fa453e1cc3a321b38d941490f9670da9ac646375b`  
		Last Modified: Fri, 02 Jun 2023 01:46:39 GMT  
		Size: 12.5 MB (12493726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d9edfe8d91f42e99880947b73dcdf5cdf32e2ee2da2b1a5ddf6953dd5c6c4e`  
		Last Modified: Fri, 02 Jun 2023 01:46:43 GMT  
		Size: 54.6 MB (54645976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a151c444d575476e86e79e9a8434d3d55c1412045220745595dc7e9d70d2f0e4`  
		Last Modified: Fri, 02 Jun 2023 01:46:37 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d93e34cf1457ec35fde213ec8fcd6c7bdaee3d690256fde7c13189785b51ec`  
		Last Modified: Sun, 04 Jun 2023 16:03:09 GMT  
		Size: 337.1 KB (337101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703c01010b9866f1834b6f7b283703c96b52dc5ca122548e6cb3efd33141604f`  
		Last Modified: Sun, 04 Jun 2023 16:03:13 GMT  
		Size: 58.8 MB (58820591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:09c43ac9dd8e55ae38571696651afa70fdb7fec2d8a240c091954eaddefed38f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153746338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f10bb02b0ed608e0f84e9088693b9d3ae36b302c4dd33991abae04b8f0e404`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:46:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:02 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Fri, 16 Jun 2023 02:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='195808eb42ab73535c84de05188914a52a47c1ac784e4bf66de95fe1fd315a5a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        armhf|arm)          ESUM='3f4848700a4bf856d3c138dc9c2b305b978879c8fbef5aa7df34a7c2fe1b64b8';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u372b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='bb85303848fe402d4f1004f748f80ccb39cb11f356f50a513555d1083c3913b8';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='78a0b3547d6f3d46227f2ad8c774248425f20f1cd63f399b713f0cdde2cc376c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 16 Jun 2023 02:46:08 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Fri, 16 Jun 2023 04:39:57 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 16 Jun 2023 04:39:57 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 16 Jun 2023 04:39:57 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:40:01 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 16 Jun 2023 04:40:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 16 Jun 2023 04:40:01 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 16 Jun 2023 04:40:19 GMT
RUN boot
# Fri, 16 Jun 2023 04:40:19 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a707fe2fc3c87da15576bd7b678fe8f2591ad481cc638b8cfe52664b47d2cf`  
		Last Modified: Fri, 16 Jun 2023 02:49:56 GMT  
		Size: 12.5 MB (12454449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d4c427d57b59d82ea1501e00ff438f2efc6f1db42e56b70350b090abbcbe07`  
		Last Modified: Fri, 16 Jun 2023 02:49:59 GMT  
		Size: 53.7 MB (53743995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f952771c8615a638a0c9898e82382b40a839b3da392841521035e9ce56bf1e20`  
		Last Modified: Fri, 16 Jun 2023 02:49:54 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3804e35c352cf88e81b0f7a57c5d4aeeab1c2f30554b5917e3bbb988700678`  
		Last Modified: Fri, 16 Jun 2023 04:52:35 GMT  
		Size: 338.0 KB (337969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9266b590c0f4b10b95679d2820910e449df0e4872a8c54f0ba16e463f1d26388`  
		Last Modified: Fri, 16 Jun 2023 04:52:38 GMT  
		Size: 58.8 MB (58820560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
