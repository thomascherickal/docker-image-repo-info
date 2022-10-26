## `clojure:temurin-11-tools-deps-1.11.1.1165-focal`

```console
$ docker pull clojure@sha256:df2448358ac5187f16feb23226e0f1f4f8ea02dc77df2d1d192ff7d7c93c6ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1165-focal` - linux; amd64

```console
$ docker pull clojure@sha256:ba61fef41b3db9ce4ae9f4a89ef2932ed3594735bf95880127b9deefa4b2df63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306052324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1baa042afb9ad1e69e58ef8428b90903e4c2b3aba1ac06489a6740aec5b62f`
-	Default Command: `["clj"]`

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
# Thu, 06 Oct 2022 03:55:19 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Thu, 06 Oct 2022 03:55:19 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:55:35 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Thu, 06 Oct 2022 03:55:35 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 06 Oct 2022 03:55:35 GMT
CMD ["clj"]
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
	-	`sha256:030f5190bf307929d09887960b36a70ed8a360030a5b7e39797b3e4302ac40d8`  
		Last Modified: Thu, 06 Oct 2022 04:11:14 GMT  
		Size: 63.0 MB (62994942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931526320fc672d0ca71834460d7d6f5f27660ca2cc2e0bb1a0e664a6f24b200`  
		Last Modified: Thu, 06 Oct 2022 04:11:05 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1165-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ad7f971b512a77e47762de168bd327eeffa1a12d996ac6ef16fb90196fde4754
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301413351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97764d5ac0088996883556ef45c8ac803a888aa083748086a06ee08ae9c129f`
-	Default Command: `["clj"]`

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
# Wed, 26 Oct 2022 15:44:11 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Wed, 26 Oct 2022 15:44:12 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:44:26 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:44:26 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 26 Oct 2022 15:44:26 GMT
CMD ["clj"]
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
	-	`sha256:307572b466227af5a3c81d4b13823d262c51a95220a7e134a669da990ced4ad1`  
		Last Modified: Wed, 26 Oct 2022 16:00:15 GMT  
		Size: 63.1 MB (63123496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5a65665a69fea7b66d1e69fdb9203dbcb10af97fed1459121112c2ac902a14`  
		Last Modified: Wed, 26 Oct 2022 16:00:09 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
