## `clojure:temurin-11-boot-jammy`

```console
$ docker pull clojure@sha256:9b949c104781599760c9f275e848281c34cd1c4fcf3b06d6c274619600b1c6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-jammy` - linux; amd64

```console
$ docker pull clojure@sha256:caca2b003b2a8bcee6ebadb1983a8236c6d81250721cc4ec760fe4d43a95e820
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300505700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113da80def5d67158cd55983bc0bfa97c53bdb4500c28a7774379fd0b1df14cd`
-	Default Command: `["boot","repl"]`

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
# Fri, 09 Dec 2022 01:43:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 18:43:59 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 24 Jan 2023 18:44:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 24 Jan 2023 18:44:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 24 Jan 2023 18:44:10 GMT
CMD ["jshell"]
# Wed, 25 Jan 2023 00:40:33 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 00:40:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 00:40:33 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:40:38 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 00:40:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 00:40:38 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 00:40:56 GMT
RUN boot
# Wed, 25 Jan 2023 00:40:56 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96aa423488f0ed1e9bf6c6da11fa7fb53568d1ea4003892416b3adeccb47e3bf`  
		Last Modified: Fri, 09 Dec 2022 01:50:02 GMT  
		Size: 12.4 MB (12432218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e9d0739b4e4d246bcb85210907656b461b7e455e8f94317955bf08c2d314`  
		Last Modified: Tue, 24 Jan 2023 18:50:50 GMT  
		Size: 198.5 MB (198487760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a77878489014a05507aa57bbd74c4fa228b99b14f5d852ab4677ca302a4673`  
		Last Modified: Tue, 24 Jan 2023 18:50:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c5e4d2f771ea8592f3592d46cacd8ba3548e389053f09385bcc64f3e037655`  
		Last Modified: Wed, 25 Jan 2023 00:54:54 GMT  
		Size: 336.4 KB (336446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec52e0be85aeb069a4fb7340c7b356949890591e257a5d28beb720d0ec543a4`  
		Last Modified: Wed, 25 Jan 2023 00:54:58 GMT  
		Size: 58.8 MB (58820395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-jammy` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:79d70a724cf01029c2380b3c3be71652e524227bf10d4fe92ddc2ddeeef273c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.2 MB (295182737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15b676e14e7a1eb2320aacc6ac440998e4d63e2b4657cbc373b9d3005de86d7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:43:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:43:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:43:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 17:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:33 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 31 Jan 2023 17:45:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 17:45:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 17:45:43 GMT
CMD ["jshell"]
# Tue, 31 Jan 2023 20:51:08 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 31 Jan 2023 20:51:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 31 Jan 2023 20:51:08 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:51:12 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 31 Jan 2023 20:51:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 31 Jan 2023 20:51:12 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 31 Jan 2023 20:51:28 GMT
RUN boot
# Tue, 31 Jan 2023 20:51:28 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6471d4f305436bdd6e09ea64bdf7a303979f4d8cdb6c9606715fc21afa9ad`  
		Last Modified: Tue, 31 Jan 2023 17:50:26 GMT  
		Size: 12.4 MB (12391264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d8e0eedc83be474a9b2366f9c420c90e3f49c24003604b9fe63731bd03e0c8`  
		Last Modified: Tue, 31 Jan 2023 17:51:44 GMT  
		Size: 195.2 MB (195247627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ce25351c32ab8a48e1e8cbfc834e00b148f1bb608f6f6c74432998feaaff91`  
		Last Modified: Tue, 31 Jan 2023 17:51:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668334d2c41c7b931503dca98def6ab196027b0245c66397d93ca9ca8cd21501`  
		Last Modified: Tue, 31 Jan 2023 21:04:55 GMT  
		Size: 338.4 KB (338400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bc7c5dda7a45a6f8d90e9a97c5105491d52af8cb7743b9ae980bd408578292`  
		Last Modified: Tue, 31 Jan 2023 21:04:58 GMT  
		Size: 58.8 MB (58820297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
