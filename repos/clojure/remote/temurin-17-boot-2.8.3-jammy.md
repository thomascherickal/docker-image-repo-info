## `clojure:temurin-17-boot-2.8.3-jammy`

```console
$ docker pull clojure@sha256:b3fc774fc01905f1065d43b2b7f932beb9ae663ce92d906909f268046687c99f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-jammy` - linux; amd64

```console
$ docker pull clojure@sha256:4e73cc37e0160c24448676089b0fa602c79dbbadb807a0c48839a8f13109f66d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.7 MB (298720187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f9f8004807b0c95ef80e1d846f78a7605d116a2fdaad7a6c694d78eb7e3d245`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:03:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:03:02 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 17:03:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:03:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 17:03:15 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 03:45:16 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 06 Oct 2022 03:45:16 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 06 Oct 2022 03:45:16 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:45:21 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 06 Oct 2022 03:45:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 06 Oct 2022 03:45:21 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 06 Oct 2022 03:46:01 GMT
RUN boot
# Thu, 06 Oct 2022 03:57:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 06 Oct 2022 03:57:41 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 06 Oct 2022 03:57:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b295fc69f17be5773c7d5e868ebc3c55b8e7789141f3aa47363fa69a7a446c7a`  
		Last Modified: Wed, 05 Oct 2022 17:10:08 GMT  
		Size: 17.0 MB (16985789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd77715f382e98938e79c50dd4e198e1ed0591a6e4d742c42ce76539de42b46`  
		Last Modified: Wed, 05 Oct 2022 17:10:20 GMT  
		Size: 192.1 MB (192145595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01940d6ad844857adae5eff7e87edb52b8913729617e44e0f36a7dab19831b2f`  
		Last Modified: Wed, 05 Oct 2022 17:10:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19fe39b3b39c67b251a3af1eb9321b112e9082384830499dc62825fe61ad50`  
		Last Modified: Thu, 06 Oct 2022 04:06:09 GMT  
		Size: 338.5 KB (338532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e5961c5832b2a418ce52e097139d6d0de81760de6f083275820b36850421be`  
		Last Modified: Thu, 06 Oct 2022 04:06:13 GMT  
		Size: 58.8 MB (58820771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2939fd9c17fdcfa9057e9fa4704af1a8b11ef8c41dc66a2b3f9b3a40a2363b4`  
		Last Modified: Thu, 06 Oct 2022 04:13:01 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-jammy` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b60fe3e29218c948a0e1ccf13deb34369429da8377a0ac3411e85a389dac6a9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296872313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671ef863434707fbff5f7dcdc4825664c898c31cb267229f6aeed0e5add07f54`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:08:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:08:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:12:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:12:19 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 26 Oct 2022 01:12:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Oct 2022 01:12:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 01:12:29 GMT
CMD ["jshell"]
# Wed, 26 Oct 2022 15:33:35 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:33:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:33:35 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:33:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:33:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:33:40 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:34:20 GMT
RUN boot
# Wed, 26 Oct 2022 15:46:23 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 15:46:23 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 15:46:23 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbcda71286ccda82b38ebdb092380175412af668b5afa39d175cd3cdefd14e4`  
		Last Modified: Wed, 26 Oct 2022 01:20:19 GMT  
		Size: 18.4 MB (18418404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f760cd96c6aa0b1d070451e5f9d8f4ecefdf4172993c4e7183465f4ffd252a`  
		Last Modified: Wed, 26 Oct 2022 01:20:29 GMT  
		Size: 190.9 MB (190911164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fe3d0d60ddcdefddd94cc47a6dcd12ab9a1fd6c41d0e10ba3dc2a85484150`  
		Last Modified: Wed, 26 Oct 2022 01:20:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edb1db28e9bf5cc3c6758bda7470fd1445d05b00549ae61ce931e2168ce41cb`  
		Last Modified: Wed, 26 Oct 2022 15:55:34 GMT  
		Size: 338.6 KB (338648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b0b6c8f175c17cee3fff9259bc721085e46d7db9120301ec3d96e74f9d586a4`  
		Last Modified: Wed, 26 Oct 2022 15:55:37 GMT  
		Size: 58.8 MB (58821040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a25a1c1e272e41aea8742e427cd195ec01c0db5cea2bc9b16679a97d1ac712`  
		Last Modified: Wed, 26 Oct 2022 16:01:54 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
