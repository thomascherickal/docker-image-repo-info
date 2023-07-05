## `sonarqube:9-developer`

```console
$ docker pull sonarqube@sha256:d231773f02bf99229353792408e96ad75c537d0f93ce66f67dcd61dc9e2e40d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:e2287947425bc684eccc631452765b40a301b61d4ca6bea24461a50c3fc6e208
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **490.2 MB (490165489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1b7c0d92e51f186cdb376eca278ca82f066f21075c33d23658dc29111034f2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/entrypoint.sh"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:33:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:33:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:33:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 20:36:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:36:31 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Tue, 04 Jul 2023 20:37:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 20:37:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 05 Jul 2023 12:19:36 GMT
LABEL org.opencontainers.image.url=https://github.com/SonarSource/docker-sonarqube
# Wed, 05 Jul 2023 12:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Jul 2023 12:19:36 GMT
ARG SONARQUBE_VERSION=9.9.1.69595
# Wed, 05 Jul 2023 12:20:00 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:00 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:20:19 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:20:19 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:20:20 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:20:20 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:20:20 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:20:20 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:20:20 GMT
ENTRYPOINT ["/opt/sonarqube/docker/entrypoint.sh"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b566cb887b5c06e04f5cd97660a99e73bd52ceb9d72c6db6383ae8470cc4cf`  
		Last Modified: Tue, 04 Jul 2023 20:41:38 GMT  
		Size: 17.0 MB (17040993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc8f3b3863b8985ba0a6078c433c2f720b393c4a85af108476993b5b1ad4bce`  
		Last Modified: Tue, 04 Jul 2023 20:42:23 GMT  
		Size: 47.0 MB (47006277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb2b830c8b634c56503567ad290d66305d253111cfc90f53a0b81826df2ce81`  
		Last Modified: Tue, 04 Jul 2023 20:42:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768f9dc791424420775b19b976a174b55522e2a60f81b946fa7d232f61e3d860`  
		Last Modified: Wed, 05 Jul 2023 12:25:08 GMT  
		Size: 395.7 MB (395686346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4df3e3919adbdecd907493abfacef36b06c086247f0f08d88b8f966524d5`  
		Last Modified: Wed, 05 Jul 2023 12:24:51 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9-developer` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:9f618d568c66c7f942586427dded2f2d6d3d5da68077bf84dc891cff3f7d2ccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.0 MB (489012396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b46fe670877ec0ffdcac6e4a4a9197ec5a2ecd15fd9e914bbdc07dcab23e9388`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/entrypoint.sh"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 15:34:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 15:34:51 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Tue, 04 Jul 2023 15:35:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 15:35:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 05 Jul 2023 04:52:10 GMT
LABEL org.opencontainers.image.url=https://github.com/SonarSource/docker-sonarqube
# Wed, 05 Jul 2023 04:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Jul 2023 04:52:10 GMT
ARG SONARQUBE_VERSION=9.9.1.69595
# Wed, 05 Jul 2023 04:52:33 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:52:33 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:53:06 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:53:08 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:53:08 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:53:08 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:53:08 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:53:08 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:53:09 GMT
ENTRYPOINT ["/opt/sonarqube/docker/entrypoint.sh"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f85d89e7da0f3af0f527e7300cced784d0ba64249b8c376690599d313cb056`  
		Last Modified: Tue, 04 Jul 2023 15:39:09 GMT  
		Size: 18.5 MB (18466568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1fcde918d2f180d437fd09c8ef6f797f4ea4708a3eb7e748a902cfa5f586f8`  
		Last Modified: Tue, 04 Jul 2023 15:39:47 GMT  
		Size: 46.5 MB (46488633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befad100d8565490272428227d229ff10ea84d74312878f1dd7605f7838dc916`  
		Last Modified: Tue, 04 Jul 2023 15:39:42 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573bad91386a1b6f67edf1de261b037d7af2e2ac0406d6b8ac980daab7d13231`  
		Last Modified: Wed, 05 Jul 2023 04:59:12 GMT  
		Size: 395.7 MB (395665546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4dc411b310755f75dcfe62608befe92bc9c21aa09b3e2c71ba09aacff96f806`  
		Last Modified: Wed, 05 Jul 2023 04:58:58 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
