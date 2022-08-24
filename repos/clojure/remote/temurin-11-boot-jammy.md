## `clojure:temurin-11-boot-jammy`

```console
$ docker pull clojure@sha256:9cf738269cc468837b36619c61b127a3adcaa71334290e114defdcdf39cfd7d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-jammy` - linux; amd64

```console
$ docker pull clojure@sha256:b658b87867a7eba96330d5ea9c39dfca40d729d7c9d0858b67da2bd1e3dd7ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300169124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cae8ebfbc348b17ec9fc7fb1b946dff7a577ed443024a785b77356b851e4290`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:20:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:20:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:20:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:20:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:20:36 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:20:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2b89cabf0ce1c2cedadd92b798d6e9056bc27c71a06f5ba24ede5dc9c316e3e8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='a703acfd04ece4a4aac4cb9bda26b7d225874008bba324237bd6f53792edb778';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b18877871eda801ccb99bb34c5d7d77fccf6adad02514110c21389632ec91024';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b16b1b50699a9caaae3d782be687625d81e069c886df904f83d13e6c4322a179';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f6b513757d386352cf91514ed5859d1ab59364b4453e1f1c57152ba2039b8e2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:20:47 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:20:47 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:49:47 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 21:49:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:49:47 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:49:51 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 21:49:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 21:49:51 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 21:50:09 GMT
RUN boot
# Wed, 24 Aug 2022 21:50:10 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65811de5a1ce73e051835187b84371fd526024c2be009224c3a1f5adaa87c90`  
		Last Modified: Fri, 12 Aug 2022 17:28:31 GMT  
		Size: 12.5 MB (12456003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852f83026af1747aab2a28e84a1cddc27b27b4ff0a58162623b5e285008a6fc`  
		Last Modified: Wed, 24 Aug 2022 19:26:42 GMT  
		Size: 198.1 MB (198130513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6965fe307ff23e50d6c80922c45a21ede484da903755a33dcae180421f6999`  
		Last Modified: Wed, 24 Aug 2022 19:26:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8069c1e3312fdb83ff59bbf5ee4b6b7e4c5e6a419331ae1e591f89c79c75ad`  
		Last Modified: Wed, 24 Aug 2022 21:57:58 GMT  
		Size: 335.8 KB (335768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb4129346de540ad7e48f36ff09d8280ad325ef90af29e8df33797087c5e581`  
		Last Modified: Wed, 24 Aug 2022 21:58:01 GMT  
		Size: 58.8 MB (58820528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-jammy` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4d4498db08f78f5132b9f38467be30ffa395e2ebdd2868177f8f4d88ee14a759
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.6 MB (294587150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe8ca8026e30c2ef53fb522a70fe5359c44298d7d8381598b9e8a1d109a0d28`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:40:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:40:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:40:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:40:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:41:05 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:41:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2b89cabf0ce1c2cedadd92b798d6e9056bc27c71a06f5ba24ede5dc9c316e3e8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='a703acfd04ece4a4aac4cb9bda26b7d225874008bba324237bd6f53792edb778';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b18877871eda801ccb99bb34c5d7d77fccf6adad02514110c21389632ec91024';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b16b1b50699a9caaae3d782be687625d81e069c886df904f83d13e6c4322a179';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f6b513757d386352cf91514ed5859d1ab59364b4453e1f1c57152ba2039b8e2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:41:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:41:17 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 20:13:17 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 20:13:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 20:13:18 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 20:13:27 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 20:13:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 20:13:29 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 20:13:42 GMT
RUN boot
# Wed, 24 Aug 2022 20:13:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a729bc90f861d8ccd964a45b6f12093afcb2172c43390409a73e938d36aa1a`  
		Last Modified: Fri, 12 Aug 2022 17:51:29 GMT  
		Size: 12.4 MB (12414351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43ee09e714415ca55decbe37e157a2e3b5b3e82588b3ead33f27bb5e5c503f1`  
		Last Modified: Wed, 24 Aug 2022 19:47:37 GMT  
		Size: 194.9 MB (194876976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26331c8f79227badad801c98c8523c50b94eec248369014760cab3bfb53a9661`  
		Last Modified: Wed, 24 Aug 2022 19:47:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28079ecacbd027323d0e60d8a2346bb227eb365da98d2ba2f396eddbb1e505fb`  
		Last Modified: Wed, 24 Aug 2022 20:22:53 GMT  
		Size: 98.8 KB (98761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2557e0730015e77ba9a7606b2f8b32f7456bfa035fe25763b68cbdf1a122ee`  
		Last Modified: Wed, 24 Aug 2022 20:22:58 GMT  
		Size: 58.8 MB (58815749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
