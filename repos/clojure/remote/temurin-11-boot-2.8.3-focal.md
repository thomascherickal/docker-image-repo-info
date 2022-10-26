## `clojure:temurin-11-boot-2.8.3-focal`

```console
$ docker pull clojure@sha256:ba63e5e741fa1efb45ab13194168cface2212ffd03f12966e6f119ce9050f315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-focal` - linux; amd64

```console
$ docker pull clojure@sha256:c1b54e7078dffb0e438ffd4f7ff93d8a9aa570668ecf6f9cdbb78646be0071c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302215255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09fc50f210305529545705545a231b89cd322bb43603d9780aac6dbcc9a650eb`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 16:59:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:01:17 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 05 Oct 2022 17:01:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2b89cabf0ce1c2cedadd92b798d6e9056bc27c71a06f5ba24ede5dc9c316e3e8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='a703acfd04ece4a4aac4cb9bda26b7d225874008bba324237bd6f53792edb778';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b18877871eda801ccb99bb34c5d7d77fccf6adad02514110c21389632ec91024';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b16b1b50699a9caaae3d782be687625d81e069c886df904f83d13e6c4322a179';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f6b513757d386352cf91514ed5859d1ab59364b4453e1f1c57152ba2039b8e2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:01:28 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 17:01:28 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 03:51:54 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 06 Oct 2022 03:51:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 06 Oct 2022 03:51:54 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:51:59 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 06 Oct 2022 03:51:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 06 Oct 2022 03:51:59 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 06 Oct 2022 03:52:24 GMT
RUN boot
# Thu, 06 Oct 2022 03:52:24 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9233a70a33bef28ffc5642770b6a9c9c03ba4c926c2c5b8a45f96403495eb671`  
		Last Modified: Wed, 05 Oct 2022 17:06:50 GMT  
		Size: 16.4 MB (16352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9375b3bbb10fbbb4fec7930871c9448ebef60a6147f1948ebe71cfbdfcb06a71`  
		Last Modified: Wed, 05 Oct 2022 17:08:20 GMT  
		Size: 198.1 MB (198129245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d2faf78e22583f22e6f1c9f76aa4e6dfb6d8bc3b98ecc014694f04f824495`  
		Last Modified: Wed, 05 Oct 2022 17:08:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98431fbc22c258fb8020043840ef2a86b58ed87d977fe18c55786db81dfcf9a`  
		Last Modified: Thu, 06 Oct 2022 04:09:04 GMT  
		Size: 337.9 KB (337866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3423bb5ac5c54ce7ce3e4a85fab06eda9cc6676c6107ee5f7cb46a6d11316c`  
		Last Modified: Thu, 06 Oct 2022 04:09:07 GMT  
		Size: 58.8 MB (58820625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:37c3ea5a894b46140958fa72b9390f86d78354ce1a30aa07a8eb6c6440f62af2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297448858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b02b854895e988636488aff7613c72192c42d74009cb3ab28f009ce90b92da`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:07:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:07:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:07:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:08:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:10:09 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 26 Oct 2022 01:10:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2b89cabf0ce1c2cedadd92b798d6e9056bc27c71a06f5ba24ede5dc9c316e3e8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='a703acfd04ece4a4aac4cb9bda26b7d225874008bba324237bd6f53792edb778';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b18877871eda801ccb99bb34c5d7d77fccf6adad02514110c21389632ec91024';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b16b1b50699a9caaae3d782be687625d81e069c886df904f83d13e6c4322a179';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f6b513757d386352cf91514ed5859d1ab59364b4453e1f1c57152ba2039b8e2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Oct 2022 01:10:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 01:10:25 GMT
CMD ["jshell"]
# Wed, 26 Oct 2022 15:39:09 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:39:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:39:10 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:39:17 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:39:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:39:17 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:39:39 GMT
RUN boot
# Wed, 26 Oct 2022 15:39:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9bffe95bbbebdbdfba5c69142aeb65478735d04064fd29982a5b9c980559e`  
		Last Modified: Wed, 26 Oct 2022 01:16:15 GMT  
		Size: 16.2 MB (16216007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8c3cca8e2bed9bb815370558027bbb061daeb97bb885f6775c5f84ecb769dc`  
		Last Modified: Wed, 26 Oct 2022 01:18:06 GMT  
		Size: 194.9 MB (194877058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adca56bcc01b8733bc9129b5c092d02e64ca44faa0f8011186c60c0857b3f45d`  
		Last Modified: Wed, 26 Oct 2022 01:17:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325f4b45354ca9e00b67e9f2745bb5fa8cb7b2939da5954bbf746b27ac3398b3`  
		Last Modified: Wed, 26 Oct 2022 15:58:14 GMT  
		Size: 339.0 KB (339048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f5b5cd435651d3c9d92dbf770fad2b9e83e3bb78db6dc826be08bac4281f16`  
		Last Modified: Wed, 26 Oct 2022 15:58:16 GMT  
		Size: 58.8 MB (58820573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
