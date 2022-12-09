## `clojure:temurin-19-boot-2.8.3-jammy`

```console
$ docker pull clojure@sha256:3e251932e1f34742c65f974f74ae6a4568e1e8556b352084ff1e58d1bb303c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-2.8.3-jammy` - linux; amd64

```console
$ docker pull clojure@sha256:2e103928cfd736febdc5ea18383eb544350273dd4a977958f89b54952ce03d97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.7 MB (307675146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4908920a9b560aa2d8be67a1153fefba391e20e14c0d1a0720e647d5c50ee49a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:45:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:47:11 GMT
ENV JAVA_VERSION=jdk-19.0.1+10
# Fri, 09 Dec 2022 01:47:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5e8d7b3189364afd78d936bad140dbe1e7025d4b96d530ed5536d035c21afb7c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='5f404ae08d7c49f22fe04c04ec39d7e7b17cae2007b9513ad1a7a1164174898b';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_arm_linux_hotspot_19.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79320712bbef13825a0aa308621006f32e54f503142737fb21ff085185a61a96';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0b4168e5a98d89b0a24fb2357b3544980d8c88a639024cde18b119b27d7583ae';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='163da7ea140210bae97c6a4590c757858ab4520a78af0e3e33129863d4087552';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_x64_linux_hotspot_19.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 01:47:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 01:47:23 GMT
CMD ["jshell"]
# Fri, 09 Dec 2022 06:46:46 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 06:46:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 06:46:46 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:46:50 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 06:46:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 06:46:50 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 06:47:07 GMT
RUN boot
# Fri, 09 Dec 2022 06:47:08 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 06:47:08 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 06:47:08 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8d923227d8dc300e1ddab1b65c83c0eff7f4a7105d958420872f7138b79735`  
		Last Modified: Fri, 09 Dec 2022 01:52:47 GMT  
		Size: 17.0 MB (16973851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4ed80f1aefd46fa11e66509942c3ee2a70f02c2d1c47426c9bad990af615ef`  
		Last Modified: Fri, 09 Dec 2022 01:54:30 GMT  
		Size: 201.1 MB (201112972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca856ce989d443c895945409dd9259e95888857878ba87bccb665f9b8c994720`  
		Last Modified: Fri, 09 Dec 2022 01:54:15 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03d1ba8bd862ded294047b787f6d56d56e827c8b52d95c57bb3fd09bdca8e5c`  
		Last Modified: Fri, 09 Dec 2022 07:00:40 GMT  
		Size: 338.6 KB (338646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73732aded8c538c1dc44d1f75066176e4cc669d42477730c1557748c71c589b`  
		Last Modified: Fri, 09 Dec 2022 07:00:43 GMT  
		Size: 58.8 MB (58820391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72223928f2563a63b5487e9d9d179eab5072fe88a70ebfa7f9b78be7367c0036`  
		Last Modified: Fri, 09 Dec 2022 07:00:40 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-2.8.3-jammy` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:95026c8b8b723bee7905930bbcce1046c4e5f70e7462ab7f4d0671a593cb50c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305809685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1c7d12b5eaaa0064b62a4b2a836010e60946bd0489cd8bd97d75656336a630`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:39:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:39:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:39:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:42:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:43:00 GMT
ENV JAVA_VERSION=jdk-19.0.1+10
# Fri, 09 Dec 2022 03:43:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5e8d7b3189364afd78d936bad140dbe1e7025d4b96d530ed5536d035c21afb7c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='5f404ae08d7c49f22fe04c04ec39d7e7b17cae2007b9513ad1a7a1164174898b';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_arm_linux_hotspot_19.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79320712bbef13825a0aa308621006f32e54f503142737fb21ff085185a61a96';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0b4168e5a98d89b0a24fb2357b3544980d8c88a639024cde18b119b27d7583ae';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='163da7ea140210bae97c6a4590c757858ab4520a78af0e3e33129863d4087552';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_x64_linux_hotspot_19.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:43:11 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 03:43:11 GMT
CMD ["jshell"]
# Fri, 09 Dec 2022 05:12:14 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 05:12:15 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 05:12:15 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:12:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 05:12:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 05:12:18 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 05:12:34 GMT
RUN boot
# Fri, 09 Dec 2022 05:12:34 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 05:12:34 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 05:12:34 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f2e5e37e706412c1481b71d2240df4fe659ef83ae4d2932a8ddfe42b0d3d20`  
		Last Modified: Fri, 09 Dec 2022 03:48:04 GMT  
		Size: 18.4 MB (18400373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254728523863be91e6c3971768a656e78c04e7d3ec2f52cfb7a75f0deb65bfa9`  
		Last Modified: Fri, 09 Dec 2022 03:49:34 GMT  
		Size: 199.9 MB (199864063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a70e08ea6acf03d88d3da9a923e594e78f1e7a821229c800d8e75ede220c9bb`  
		Last Modified: Fri, 09 Dec 2022 03:49:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59997d6c5a3546ac68753cac36e2f846fbb25f419de0136e1ac98cce197c00a`  
		Last Modified: Fri, 09 Dec 2022 05:24:51 GMT  
		Size: 340.0 KB (339989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6d9c6771c541cc4c04ea902c3b9756ff8bed6d6b7e3150984d28fde7c54147`  
		Last Modified: Fri, 09 Dec 2022 05:24:54 GMT  
		Size: 58.8 MB (58820211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ba8e46fc60ae0cce2eacfdeb0662be8f3fa16e1873babbf6fc012319f3c8ed`  
		Last Modified: Fri, 09 Dec 2022 05:24:51 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
