## `clojure:boot-2.8.3-focal`

```console
$ docker pull clojure@sha256:b97b09128e81cf49425251974771f13900bb5c77878d62dec172328a5f740be3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:boot-2.8.3-focal` - linux; amd64

```console
$ docker pull clojure@sha256:77ef06ee579bc8581bec211eeaa430ecb3da7e04e295197d65ceacc78ebaa8b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.0 MB (300000107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6b1c94e463c7822da47cb021a1afe8ac9d67b938e111cf2abbce187ca4c716`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:19:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:23:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:22:07 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:22:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:22:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:22:31 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:52:32 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 21:52:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:52:32 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:52:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 21:52:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 21:52:37 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 21:52:54 GMT
RUN boot
# Wed, 24 Aug 2022 21:52:54 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 21:52:54 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 21:52:54 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff450785d414a328de85b6a3efa41eb49c35822535ae4c97558901c3c68dc5a1`  
		Last Modified: Fri, 12 Aug 2022 17:32:12 GMT  
		Size: 20.1 MB (20120218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6051a9992bc52acd3cdd8b3d914563b5a896d4d9b0f8bbc44a9cc6b604d43`  
		Last Modified: Wed, 24 Aug 2022 19:29:17 GMT  
		Size: 192.1 MB (192145944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6852eadfb5ca048ed11a12941582af6aa0f2c5bbb657c1d17da0432cca956`  
		Last Modified: Wed, 24 Aug 2022 19:29:03 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1462815d777b50466767f4a0a0b892e9c997afd1e27bd36883f098ab684838b`  
		Last Modified: Wed, 24 Aug 2022 22:00:16 GMT  
		Size: 340.2 KB (340222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0c3cead37641f6b66cfa5bdd8b6c6be4c04655f0be62d68139254f86af1cf`  
		Last Modified: Wed, 24 Aug 2022 22:00:19 GMT  
		Size: 58.8 MB (58820553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3a9b3a1b2702b4ce6470ada595819d3c433ce49ade8a618951357a23520429`  
		Last Modified: Wed, 24 Aug 2022 22:00:15 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:boot-2.8.3-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0b67a4aa7ea1d87d316e863bc518b59298303bcb5a2cf051f390e2d9b85489bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297862353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11af6a5299504141d5cc0f411f141c9b0c145ba21c5747b53ab61f825619637`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:39:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:39:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:39:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:44:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:42:14 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:42:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:42:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:42:33 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 20:15:51 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 20:15:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 20:15:52 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 20:15:59 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 20:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 20:16:01 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 20:16:15 GMT
RUN boot
# Wed, 24 Aug 2022 20:16:16 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 20:16:16 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 20:16:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8c0ceb097615de30aaa4bce5d78e683a09d3766624f531951238f11979cc7f`  
		Last Modified: Fri, 12 Aug 2022 17:55:33 GMT  
		Size: 20.8 MB (20839019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5ce586470e708a85551aff42fc396cd685bbfec1da65b08353946a55a7b2d2`  
		Last Modified: Wed, 24 Aug 2022 19:49:31 GMT  
		Size: 190.9 MB (190911717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16045745fcc8bef66b5a239924807d14f1343126bbcc5a7608dcb0ca4e176d5`  
		Last Modified: Wed, 24 Aug 2022 19:49:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6782d817e9d7b1ffbe682f8535235f2efe57beeb8bffc6a6f424e6c18f69e6`  
		Last Modified: Wed, 24 Aug 2022 20:24:48 GMT  
		Size: 103.6 KB (103603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d3c13e4a7f150f70bbc05cbcea46f729e7d7dda9ad81854055f0a14aaac9b7`  
		Last Modified: Wed, 24 Aug 2022 20:24:52 GMT  
		Size: 58.8 MB (58815650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61c6d51c5218721c6d0266ee347b17ac34ca8066183a12344b1f79762996f2`  
		Last Modified: Wed, 24 Aug 2022 20:24:48 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
