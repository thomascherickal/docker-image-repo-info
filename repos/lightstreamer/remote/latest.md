## `lightstreamer:latest`

```console
$ docker pull lightstreamer@sha256:9a8b0b9be5f1e2d743e7b1f03e659bf3b96fe8acb8c034fd4b68241ee8bf25f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:latest` - linux; amd64

```console
$ docker pull lightstreamer@sha256:2b1edc2be3f96288167e293fb4695e330a919bc52169480a73f5790f80b650bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302424812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19710e06ada2812ee478808c82c1429be56209f650e155b9884f7479c359f9e7`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:43:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:43:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:43:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:44:43 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 02 Nov 2022 18:44:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2b89cabf0ce1c2cedadd92b798d6e9056bc27c71a06f5ba24ede5dc9c316e3e8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='a703acfd04ece4a4aac4cb9bda26b7d225874008bba324237bd6f53792edb778';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b18877871eda801ccb99bb34c5d7d77fccf6adad02514110c21389632ec91024';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b16b1b50699a9caaae3d782be687625d81e069c886df904f83d13e6c4322a179';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f6b513757d386352cf91514ed5859d1ab59364b4453e1f1c57152ba2039b8e2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 02 Nov 2022 18:44:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 02 Nov 2022 18:44:55 GMT
CMD ["jshell"]
# Wed, 02 Nov 2022 21:19:37 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Wed, 02 Nov 2022 21:19:43 GMT
RUN apt-get -y update         && apt-get -y install gnupg         && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:19:44 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Wed, 02 Nov 2022 21:20:38 GMT
ENV LIGHTSTREAMER_VERSION=7.3.0
# Wed, 02 Nov 2022 21:20:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.3.0/Lightstreamer-7.3.0.tar.gz
# Wed, 02 Nov 2022 21:20:41 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Wed, 02 Nov 2022 21:20:41 GMT
USER lightstreamer
# Wed, 02 Nov 2022 21:20:42 GMT
EXPOSE 8080
# Wed, 02 Nov 2022 21:20:42 GMT
WORKDIR /lightstreamer/bin/unix-like
# Wed, 02 Nov 2022 21:20:42 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af73a17c4f87e35cb9b0b52602dde1f66c242f14b489c53e0a04b737f4fa13f`  
		Last Modified: Wed, 02 Nov 2022 18:49:39 GMT  
		Size: 198.1 MB (198130544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3968368483c88b2c9a76ba7ac14216b3863cb6bc8c63cd5a101f863245d10f`  
		Last Modified: Wed, 02 Nov 2022 18:49:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98a802dd2eafe472eab7f7cec14a9c71a274d5fc3c5cec86422eb61e7d2f66d`  
		Last Modified: Wed, 02 Nov 2022 21:22:27 GMT  
		Size: 3.6 MB (3597052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5fd9ff22128c0ba7336e929614edbb689499879206844de8931e87e9f8d172`  
		Last Modified: Wed, 02 Nov 2022 21:22:26 GMT  
		Size: 2.4 KB (2396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e0ea712a64c070f36d34ceca283191e303b68ac706641635cf5d95dad88ce9`  
		Last Modified: Wed, 02 Nov 2022 21:24:35 GMT  
		Size: 57.8 MB (57830032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:latest` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:fdffa2f5c76b71e52179cfc93f39e8f4d803cca7c31ba7b92f1eba372b263b09
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297059071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1bbb54e172481c372337c776721e2bad26cebab93ac8ce89e3f40e4fbe56690`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:44:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 19:44:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 19:44:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:44:58 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 02 Nov 2022 19:45:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2b89cabf0ce1c2cedadd92b798d6e9056bc27c71a06f5ba24ede5dc9c316e3e8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='a703acfd04ece4a4aac4cb9bda26b7d225874008bba324237bd6f53792edb778';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b18877871eda801ccb99bb34c5d7d77fccf6adad02514110c21389632ec91024';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b16b1b50699a9caaae3d782be687625d81e069c886df904f83d13e6c4322a179';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f6b513757d386352cf91514ed5859d1ab59364b4453e1f1c57152ba2039b8e2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 02 Nov 2022 19:45:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 02 Nov 2022 19:45:17 GMT
CMD ["jshell"]
# Wed, 02 Nov 2022 21:54:18 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Wed, 02 Nov 2022 21:54:22 GMT
RUN apt-get -y update         && apt-get -y install gnupg         && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:54:23 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Wed, 02 Nov 2022 21:54:56 GMT
ENV LIGHTSTREAMER_VERSION=7.3.0
# Wed, 02 Nov 2022 21:54:56 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.3.0/Lightstreamer-7.3.0.tar.gz
# Wed, 02 Nov 2022 21:54:59 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Wed, 02 Nov 2022 21:54:59 GMT
USER lightstreamer
# Wed, 02 Nov 2022 21:54:59 GMT
EXPOSE 8080
# Wed, 02 Nov 2022 21:54:59 GMT
WORKDIR /lightstreamer/bin/unix-like
# Wed, 02 Nov 2022 21:54:59 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5b9524848e4c82e9918b970ac0b0a25710fc47af27f8766521c11b17bc7dff`  
		Last Modified: Wed, 02 Nov 2022 19:49:16 GMT  
		Size: 194.9 MB (194877760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae989b6a0d38ef7ddd5c21eb689ef22be729f406420665f8964f9cf830bf5a9b`  
		Last Modified: Wed, 02 Nov 2022 19:49:04 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7137ecde6292b74badc2741e7e4b133b83cb71a2aa637dc8dd8044d9c0f89b`  
		Last Modified: Wed, 02 Nov 2022 21:56:42 GMT  
		Size: 3.6 MB (3570287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b318bffcc96db2084aed18a292325aa34cd563a41306601de86b63ac7257974c`  
		Last Modified: Wed, 02 Nov 2022 21:56:42 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c6d96a2e028e62c238e46c07255056d79c5ae6de2cbfbaede6af30c9fedf78`  
		Last Modified: Wed, 02 Nov 2022 21:58:53 GMT  
		Size: 57.8 MB (57829970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
