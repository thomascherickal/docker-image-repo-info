<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sonarqube`

-	[`sonarqube:10-community`](#sonarqube10-community)
-	[`sonarqube:10-datacenter-app`](#sonarqube10-datacenter-app)
-	[`sonarqube:10-datacenter-search`](#sonarqube10-datacenter-search)
-	[`sonarqube:10-developer`](#sonarqube10-developer)
-	[`sonarqube:10-enterprise`](#sonarqube10-enterprise)
-	[`sonarqube:10.1-community`](#sonarqube101-community)
-	[`sonarqube:10.1-datacenter-app`](#sonarqube101-datacenter-app)
-	[`sonarqube:10.1-datacenter-search`](#sonarqube101-datacenter-search)
-	[`sonarqube:10.1-developer`](#sonarqube101-developer)
-	[`sonarqube:10.1-enterprise`](#sonarqube101-enterprise)
-	[`sonarqube:10.1.0-community`](#sonarqube1010-community)
-	[`sonarqube:10.1.0-datacenter-app`](#sonarqube1010-datacenter-app)
-	[`sonarqube:10.1.0-datacenter-search`](#sonarqube1010-datacenter-search)
-	[`sonarqube:10.1.0-developer`](#sonarqube1010-developer)
-	[`sonarqube:10.1.0-enterprise`](#sonarqube1010-enterprise)
-	[`sonarqube:9-community`](#sonarqube9-community)
-	[`sonarqube:9-datacenter-app`](#sonarqube9-datacenter-app)
-	[`sonarqube:9-datacenter-search`](#sonarqube9-datacenter-search)
-	[`sonarqube:9-developer`](#sonarqube9-developer)
-	[`sonarqube:9-enterprise`](#sonarqube9-enterprise)
-	[`sonarqube:9.9-community`](#sonarqube99-community)
-	[`sonarqube:9.9-datacenter-app`](#sonarqube99-datacenter-app)
-	[`sonarqube:9.9-datacenter-search`](#sonarqube99-datacenter-search)
-	[`sonarqube:9.9-developer`](#sonarqube99-developer)
-	[`sonarqube:9.9-enterprise`](#sonarqube99-enterprise)
-	[`sonarqube:9.9.1-community`](#sonarqube991-community)
-	[`sonarqube:9.9.1-datacenter-app`](#sonarqube991-datacenter-app)
-	[`sonarqube:9.9.1-datacenter-search`](#sonarqube991-datacenter-search)
-	[`sonarqube:9.9.1-developer`](#sonarqube991-developer)
-	[`sonarqube:9.9.1-enterprise`](#sonarqube991-enterprise)
-	[`sonarqube:community`](#sonarqubecommunity)
-	[`sonarqube:datacenter-app`](#sonarqubedatacenter-app)
-	[`sonarqube:datacenter-search`](#sonarqubedatacenter-search)
-	[`sonarqube:developer`](#sonarqubedeveloper)
-	[`sonarqube:enterprise`](#sonarqubeenterprise)
-	[`sonarqube:latest`](#sonarqubelatest)
-	[`sonarqube:lts`](#sonarqubelts)
-	[`sonarqube:lts-community`](#sonarqubelts-community)
-	[`sonarqube:lts-datacenter-app`](#sonarqubelts-datacenter-app)
-	[`sonarqube:lts-datacenter-search`](#sonarqubelts-datacenter-search)
-	[`sonarqube:lts-developer`](#sonarqubelts-developer)
-	[`sonarqube:lts-enterprise`](#sonarqubelts-enterprise)

## `sonarqube:10-community`

```console
$ docker pull sonarqube@sha256:b0e9f03c5c1b9faf2c4cc3bbd81ef90d9df8876e9b40271881a6168774374c6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:0f225682c2db92dd38514bddbed0bf2240a09386686d4462752dce91da594eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **468.4 MB (468359493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907b1b7b82bee77ada1c7170a6f72b871c806fc1a0e97d8e77490b7121c989e4`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:21:41 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:21:59 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:00 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:00 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:00 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:00 GMT
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
	-	`sha256:394329c8ee57507abde6133e4be41035dc28322b8d5784283c5c265bae0c8bee`  
		Last Modified: Wed, 05 Jul 2023 12:27:11 GMT  
		Size: 373.9 MB (373880354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c43f2deaf333887421a0851e818b61bfdde26ce80e2e1a4ab12ba7b0e45e7f`  
		Last Modified: Wed, 05 Jul 2023 12:26:55 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:89e3f27f2cc0c79aceb8c9e5f6e468cecffe3f90fe7eb7a3d599673fbd8681ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467198578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294c1b266c52c9dc89ba5c29465f3acf2c071526cbb311a6f88f2f957283ea56`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:54:57 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:15 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:18 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:18 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:18 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:18 GMT
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
	-	`sha256:3d6b64d2c7bbcaefb52364635d1548c284e9117ed6efbd12505e2a237f543f5d`  
		Last Modified: Wed, 05 Jul 2023 05:01:06 GMT  
		Size: 373.9 MB (373851726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8879d10617e8a246b0d1b696480ef4b420eb9025f14e5d811a11a7d3aa4fd`  
		Last Modified: Wed, 05 Jul 2023 05:00:52 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10-datacenter-app`

```console
$ docker pull sonarqube@sha256:6e618f16f4e44f4dc893fb6787bd36a3aae6f16e9481fa7a7dc0a9242e52f1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:e4bd05d466fbd0b9b66c11e1990cf8c28169e8e38e595f50144915a1c9d1d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab37611fc601ab5f15c2eeb8de910e5aeb7c972d45437d62ece416701bd836a`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:58 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:19 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:20 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:20 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:20 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:20 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:21 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:21 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:21 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1a19a5a15e046b51dba9c274327dd2d4a6d061e6502370af23e3e199ca2981d4`  
		Last Modified: Wed, 05 Jul 2023 12:28:56 GMT  
		Size: 489.9 MB (489892103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499fdd0a44f41578c3f19fcfda431fcaf7ff5de1a51b0f22c978fb27139323f9`  
		Last Modified: Wed, 05 Jul 2023 12:28:35 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:fa566713c02911b39b4cbd5515e420aedcbd322cddee39e7e9cc7ebad9960e6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e66559188e80a0798a8f37b45c4313bd6d602beee0d53be08a4508467a7f96f`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:56:36 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:12 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:16 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:16 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:16 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:16 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:16 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:401cd866db1db244a28a6ea3dca1eb3552c1fe6bc03add294ccc23a7d3862ca9`  
		Last Modified: Wed, 05 Jul 2023 05:02:38 GMT  
		Size: 489.9 MB (489883219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b386629d530bc4be285e300df11a14a3a51b828e566f85566d0fe1ee39dfaa1`  
		Last Modified: Wed, 05 Jul 2023 05:02:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10-datacenter-search`

```console
$ docker pull sonarqube@sha256:960f362615b5eff3d5ab194a547bc2a826d21fd68c6de5a0fade1e97883767e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:d1c1e4561863f74ce6a50bd154017f4cf41567f628e2b26838ad1ff4d4c70016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73745fb21b7da208e5feb707787ff0a09aa1bcdac9fc940416c58a22a873b0fd`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:23:27 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:48 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:50 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:50 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:50 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:50 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:50 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:cd46c70cb09fa784a36370697038d617deb109c9f68de0b5e5c3a90b0d94c026`  
		Last Modified: Wed, 05 Jul 2023 12:29:29 GMT  
		Size: 489.9 MB (489892014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10558e306e9893095b53fd9dc8f767b7ba0610457756aeeb15d7167a78368dde`  
		Last Modified: Wed, 05 Jul 2023 12:29:08 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dac3679f797bfa190f5c37b028d202e74724ea79adbd6391e3e8d3233f1b6ba8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:602b8be520c0e71f321f7bb48123afbc67426e41d9022f8afe1ed762f12eb6f2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:57:24 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:53 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:57 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:57 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:57 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:57 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:57 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:75115b4064ce43511001eb98c1d542db9257cb93e39dc932a702078f33220691`  
		Last Modified: Wed, 05 Jul 2023 05:03:09 GMT  
		Size: 489.9 MB (489883187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8375ad97f4ec6161b377ff8c8af6a2d479e86e43a221aa5b27eb7ddbb44272`  
		Last Modified: Wed, 05 Jul 2023 05:02:51 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10-developer`

```console
$ docker pull sonarqube@sha256:04c0882d01c2ccf9e4eb7c43c9734987dca083599cb9926c403c41e0ab9ec61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:04d8ba491263a8391721448ebe847ac67ed0b2f4106f7952d66e10d9fee3186d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.4 MB (563384649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef08e724cfe7dfc2b2b3142a72fc7372c68466bf49b37a2f5a583a952efe504c`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:05 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:06 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:25 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:26 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:26 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:26 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:27 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:27 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:27 GMT
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
	-	`sha256:8066a59c1bbd3583352b0b54ee0b323e7839f03fbfe4e24c3c69ce7d282a095a`  
		Last Modified: Wed, 05 Jul 2023 12:27:48 GMT  
		Size: 468.9 MB (468905509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b140a90a298d12f2681656f58b556cb7e6ca6529c259ad1882dc04c53be712`  
		Last Modified: Wed, 05 Jul 2023 12:27:25 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10-developer` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:63a2db596e0a79fdc086a54af2c7d1999749fe9348bda250f8e804f26abb43e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.2 MB (562234162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d15abcb1eddfb6fb55b91a48996b9df904445cb8452ff8a39e0137cbb81b376`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:20 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:20 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:39 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:42 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:42 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:42 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:42 GMT
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
	-	`sha256:6c79339b9b2b6885c214417e76cbd4c9c8b40138f738d676d875e42621f2a386`  
		Last Modified: Wed, 05 Jul 2023 05:01:38 GMT  
		Size: 468.9 MB (468887312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb254725b1b44ca37f9c4dd1ef91a6671f1fb93c6dae8e868c4b1a52bca0c39`  
		Last Modified: Wed, 05 Jul 2023 05:01:21 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10-enterprise`

```console
$ docker pull sonarqube@sha256:6c042122eead371f181fff91a777dcc48bccf3351d7bfbacd4a4c548ac20cc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:35fe3b6a46135100a3dc72b3e7ea18fe5d5b3959e34ef0d25796d95c234d3a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.7 MB (582679450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3e99d5970b424fb459824593f5e9f16b0f3666d1e8a888a933e18ce56747a`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:30 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:30 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:50 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:51 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:51 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:52 GMT
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
	-	`sha256:97dc6fffa26b5098e6e70351cb4bb0637d2c949686e15f77513650b39d46ea47`  
		Last Modified: Wed, 05 Jul 2023 12:28:21 GMT  
		Size: 488.2 MB (488200311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a2fd8aed8319f291cb298c7bcd000cad1f32f21ec7b0a61a800592d03077bf`  
		Last Modified: Wed, 05 Jul 2023 12:28:01 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:558f2d23ade2903aaccd3be190b4466c5ad7430e7538e5564f78eaac864a5eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.5 MB (581528720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9055674352aaa3245776b65d1d235b6d5ca440c63e6d47e1c3f953d2a6c39114`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:48 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:56:24 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:56:28 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:56:28 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:56:28 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:56:28 GMT
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
	-	`sha256:09af0d1bb681e0a7877489253a8c5c13161b5c43f87a36dd802b65ea640667d4`  
		Last Modified: Wed, 05 Jul 2023 05:02:08 GMT  
		Size: 488.2 MB (488181869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc199f6b625587da3609df62174b04bc0ff8b7315b7b0e1333baa4afd83e7eb`  
		Last Modified: Wed, 05 Jul 2023 05:01:51 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1-community`

```console
$ docker pull sonarqube@sha256:b0e9f03c5c1b9faf2c4cc3bbd81ef90d9df8876e9b40271881a6168774374c6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:0f225682c2db92dd38514bddbed0bf2240a09386686d4462752dce91da594eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **468.4 MB (468359493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907b1b7b82bee77ada1c7170a6f72b871c806fc1a0e97d8e77490b7121c989e4`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:21:41 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:21:59 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:00 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:00 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:00 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:00 GMT
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
	-	`sha256:394329c8ee57507abde6133e4be41035dc28322b8d5784283c5c265bae0c8bee`  
		Last Modified: Wed, 05 Jul 2023 12:27:11 GMT  
		Size: 373.9 MB (373880354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c43f2deaf333887421a0851e818b61bfdde26ce80e2e1a4ab12ba7b0e45e7f`  
		Last Modified: Wed, 05 Jul 2023 12:26:55 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:89e3f27f2cc0c79aceb8c9e5f6e468cecffe3f90fe7eb7a3d599673fbd8681ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467198578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294c1b266c52c9dc89ba5c29465f3acf2c071526cbb311a6f88f2f957283ea56`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:54:57 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:15 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:18 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:18 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:18 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:18 GMT
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
	-	`sha256:3d6b64d2c7bbcaefb52364635d1548c284e9117ed6efbd12505e2a237f543f5d`  
		Last Modified: Wed, 05 Jul 2023 05:01:06 GMT  
		Size: 373.9 MB (373851726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8879d10617e8a246b0d1b696480ef4b420eb9025f14e5d811a11a7d3aa4fd`  
		Last Modified: Wed, 05 Jul 2023 05:00:52 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1-datacenter-app`

```console
$ docker pull sonarqube@sha256:6e618f16f4e44f4dc893fb6787bd36a3aae6f16e9481fa7a7dc0a9242e52f1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:e4bd05d466fbd0b9b66c11e1990cf8c28169e8e38e595f50144915a1c9d1d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab37611fc601ab5f15c2eeb8de910e5aeb7c972d45437d62ece416701bd836a`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:58 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:19 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:20 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:20 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:20 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:20 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:21 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:21 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:21 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1a19a5a15e046b51dba9c274327dd2d4a6d061e6502370af23e3e199ca2981d4`  
		Last Modified: Wed, 05 Jul 2023 12:28:56 GMT  
		Size: 489.9 MB (489892103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499fdd0a44f41578c3f19fcfda431fcaf7ff5de1a51b0f22c978fb27139323f9`  
		Last Modified: Wed, 05 Jul 2023 12:28:35 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:fa566713c02911b39b4cbd5515e420aedcbd322cddee39e7e9cc7ebad9960e6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e66559188e80a0798a8f37b45c4313bd6d602beee0d53be08a4508467a7f96f`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:56:36 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:12 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:16 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:16 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:16 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:16 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:16 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:401cd866db1db244a28a6ea3dca1eb3552c1fe6bc03add294ccc23a7d3862ca9`  
		Last Modified: Wed, 05 Jul 2023 05:02:38 GMT  
		Size: 489.9 MB (489883219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b386629d530bc4be285e300df11a14a3a51b828e566f85566d0fe1ee39dfaa1`  
		Last Modified: Wed, 05 Jul 2023 05:02:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1-datacenter-search`

```console
$ docker pull sonarqube@sha256:960f362615b5eff3d5ab194a547bc2a826d21fd68c6de5a0fade1e97883767e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:d1c1e4561863f74ce6a50bd154017f4cf41567f628e2b26838ad1ff4d4c70016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73745fb21b7da208e5feb707787ff0a09aa1bcdac9fc940416c58a22a873b0fd`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:23:27 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:48 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:50 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:50 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:50 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:50 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:50 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:cd46c70cb09fa784a36370697038d617deb109c9f68de0b5e5c3a90b0d94c026`  
		Last Modified: Wed, 05 Jul 2023 12:29:29 GMT  
		Size: 489.9 MB (489892014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10558e306e9893095b53fd9dc8f767b7ba0610457756aeeb15d7167a78368dde`  
		Last Modified: Wed, 05 Jul 2023 12:29:08 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dac3679f797bfa190f5c37b028d202e74724ea79adbd6391e3e8d3233f1b6ba8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:602b8be520c0e71f321f7bb48123afbc67426e41d9022f8afe1ed762f12eb6f2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:57:24 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:53 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:57 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:57 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:57 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:57 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:57 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:75115b4064ce43511001eb98c1d542db9257cb93e39dc932a702078f33220691`  
		Last Modified: Wed, 05 Jul 2023 05:03:09 GMT  
		Size: 489.9 MB (489883187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8375ad97f4ec6161b377ff8c8af6a2d479e86e43a221aa5b27eb7ddbb44272`  
		Last Modified: Wed, 05 Jul 2023 05:02:51 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1-developer`

```console
$ docker pull sonarqube@sha256:04c0882d01c2ccf9e4eb7c43c9734987dca083599cb9926c403c41e0ab9ec61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:04d8ba491263a8391721448ebe847ac67ed0b2f4106f7952d66e10d9fee3186d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.4 MB (563384649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef08e724cfe7dfc2b2b3142a72fc7372c68466bf49b37a2f5a583a952efe504c`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:05 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:06 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:25 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:26 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:26 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:26 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:27 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:27 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:27 GMT
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
	-	`sha256:8066a59c1bbd3583352b0b54ee0b323e7839f03fbfe4e24c3c69ce7d282a095a`  
		Last Modified: Wed, 05 Jul 2023 12:27:48 GMT  
		Size: 468.9 MB (468905509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b140a90a298d12f2681656f58b556cb7e6ca6529c259ad1882dc04c53be712`  
		Last Modified: Wed, 05 Jul 2023 12:27:25 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1-developer` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:63a2db596e0a79fdc086a54af2c7d1999749fe9348bda250f8e804f26abb43e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.2 MB (562234162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d15abcb1eddfb6fb55b91a48996b9df904445cb8452ff8a39e0137cbb81b376`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:20 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:20 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:39 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:42 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:42 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:42 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:42 GMT
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
	-	`sha256:6c79339b9b2b6885c214417e76cbd4c9c8b40138f738d676d875e42621f2a386`  
		Last Modified: Wed, 05 Jul 2023 05:01:38 GMT  
		Size: 468.9 MB (468887312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb254725b1b44ca37f9c4dd1ef91a6671f1fb93c6dae8e868c4b1a52bca0c39`  
		Last Modified: Wed, 05 Jul 2023 05:01:21 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1-enterprise`

```console
$ docker pull sonarqube@sha256:6c042122eead371f181fff91a777dcc48bccf3351d7bfbacd4a4c548ac20cc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:35fe3b6a46135100a3dc72b3e7ea18fe5d5b3959e34ef0d25796d95c234d3a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.7 MB (582679450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3e99d5970b424fb459824593f5e9f16b0f3666d1e8a888a933e18ce56747a`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:30 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:30 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:50 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:51 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:51 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:52 GMT
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
	-	`sha256:97dc6fffa26b5098e6e70351cb4bb0637d2c949686e15f77513650b39d46ea47`  
		Last Modified: Wed, 05 Jul 2023 12:28:21 GMT  
		Size: 488.2 MB (488200311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a2fd8aed8319f291cb298c7bcd000cad1f32f21ec7b0a61a800592d03077bf`  
		Last Modified: Wed, 05 Jul 2023 12:28:01 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:558f2d23ade2903aaccd3be190b4466c5ad7430e7538e5564f78eaac864a5eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.5 MB (581528720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9055674352aaa3245776b65d1d235b6d5ca440c63e6d47e1c3f953d2a6c39114`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:48 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:56:24 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:56:28 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:56:28 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:56:28 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:56:28 GMT
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
	-	`sha256:09af0d1bb681e0a7877489253a8c5c13161b5c43f87a36dd802b65ea640667d4`  
		Last Modified: Wed, 05 Jul 2023 05:02:08 GMT  
		Size: 488.2 MB (488181869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc199f6b625587da3609df62174b04bc0ff8b7315b7b0e1333baa4afd83e7eb`  
		Last Modified: Wed, 05 Jul 2023 05:01:51 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1.0-community`

```console
$ docker pull sonarqube@sha256:b0e9f03c5c1b9faf2c4cc3bbd81ef90d9df8876e9b40271881a6168774374c6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1.0-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:0f225682c2db92dd38514bddbed0bf2240a09386686d4462752dce91da594eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **468.4 MB (468359493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907b1b7b82bee77ada1c7170a6f72b871c806fc1a0e97d8e77490b7121c989e4`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:21:41 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:21:59 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:00 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:00 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:00 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:00 GMT
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
	-	`sha256:394329c8ee57507abde6133e4be41035dc28322b8d5784283c5c265bae0c8bee`  
		Last Modified: Wed, 05 Jul 2023 12:27:11 GMT  
		Size: 373.9 MB (373880354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c43f2deaf333887421a0851e818b61bfdde26ce80e2e1a4ab12ba7b0e45e7f`  
		Last Modified: Wed, 05 Jul 2023 12:26:55 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1.0-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:89e3f27f2cc0c79aceb8c9e5f6e468cecffe3f90fe7eb7a3d599673fbd8681ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467198578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294c1b266c52c9dc89ba5c29465f3acf2c071526cbb311a6f88f2f957283ea56`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:54:57 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:15 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:18 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:18 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:18 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:18 GMT
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
	-	`sha256:3d6b64d2c7bbcaefb52364635d1548c284e9117ed6efbd12505e2a237f543f5d`  
		Last Modified: Wed, 05 Jul 2023 05:01:06 GMT  
		Size: 373.9 MB (373851726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8879d10617e8a246b0d1b696480ef4b420eb9025f14e5d811a11a7d3aa4fd`  
		Last Modified: Wed, 05 Jul 2023 05:00:52 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1.0-datacenter-app`

```console
$ docker pull sonarqube@sha256:6e618f16f4e44f4dc893fb6787bd36a3aae6f16e9481fa7a7dc0a9242e52f1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1.0-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:e4bd05d466fbd0b9b66c11e1990cf8c28169e8e38e595f50144915a1c9d1d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab37611fc601ab5f15c2eeb8de910e5aeb7c972d45437d62ece416701bd836a`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:58 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:19 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:20 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:20 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:20 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:20 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:21 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:21 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:21 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1a19a5a15e046b51dba9c274327dd2d4a6d061e6502370af23e3e199ca2981d4`  
		Last Modified: Wed, 05 Jul 2023 12:28:56 GMT  
		Size: 489.9 MB (489892103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499fdd0a44f41578c3f19fcfda431fcaf7ff5de1a51b0f22c978fb27139323f9`  
		Last Modified: Wed, 05 Jul 2023 12:28:35 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1.0-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:fa566713c02911b39b4cbd5515e420aedcbd322cddee39e7e9cc7ebad9960e6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e66559188e80a0798a8f37b45c4313bd6d602beee0d53be08a4508467a7f96f`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:56:36 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:12 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:16 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:16 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:16 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:16 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:16 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:401cd866db1db244a28a6ea3dca1eb3552c1fe6bc03add294ccc23a7d3862ca9`  
		Last Modified: Wed, 05 Jul 2023 05:02:38 GMT  
		Size: 489.9 MB (489883219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b386629d530bc4be285e300df11a14a3a51b828e566f85566d0fe1ee39dfaa1`  
		Last Modified: Wed, 05 Jul 2023 05:02:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1.0-datacenter-search`

```console
$ docker pull sonarqube@sha256:960f362615b5eff3d5ab194a547bc2a826d21fd68c6de5a0fade1e97883767e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1.0-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:d1c1e4561863f74ce6a50bd154017f4cf41567f628e2b26838ad1ff4d4c70016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73745fb21b7da208e5feb707787ff0a09aa1bcdac9fc940416c58a22a873b0fd`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:23:27 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:48 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:50 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:50 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:50 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:50 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:50 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:cd46c70cb09fa784a36370697038d617deb109c9f68de0b5e5c3a90b0d94c026`  
		Last Modified: Wed, 05 Jul 2023 12:29:29 GMT  
		Size: 489.9 MB (489892014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10558e306e9893095b53fd9dc8f767b7ba0610457756aeeb15d7167a78368dde`  
		Last Modified: Wed, 05 Jul 2023 12:29:08 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1.0-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dac3679f797bfa190f5c37b028d202e74724ea79adbd6391e3e8d3233f1b6ba8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:602b8be520c0e71f321f7bb48123afbc67426e41d9022f8afe1ed762f12eb6f2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:57:24 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:53 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:57 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:57 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:57 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:57 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:57 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:75115b4064ce43511001eb98c1d542db9257cb93e39dc932a702078f33220691`  
		Last Modified: Wed, 05 Jul 2023 05:03:09 GMT  
		Size: 489.9 MB (489883187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8375ad97f4ec6161b377ff8c8af6a2d479e86e43a221aa5b27eb7ddbb44272`  
		Last Modified: Wed, 05 Jul 2023 05:02:51 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1.0-developer`

```console
$ docker pull sonarqube@sha256:04c0882d01c2ccf9e4eb7c43c9734987dca083599cb9926c403c41e0ab9ec61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1.0-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:04d8ba491263a8391721448ebe847ac67ed0b2f4106f7952d66e10d9fee3186d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.4 MB (563384649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef08e724cfe7dfc2b2b3142a72fc7372c68466bf49b37a2f5a583a952efe504c`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:05 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:06 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:25 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:26 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:26 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:26 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:27 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:27 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:27 GMT
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
	-	`sha256:8066a59c1bbd3583352b0b54ee0b323e7839f03fbfe4e24c3c69ce7d282a095a`  
		Last Modified: Wed, 05 Jul 2023 12:27:48 GMT  
		Size: 468.9 MB (468905509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b140a90a298d12f2681656f58b556cb7e6ca6529c259ad1882dc04c53be712`  
		Last Modified: Wed, 05 Jul 2023 12:27:25 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1.0-developer` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:63a2db596e0a79fdc086a54af2c7d1999749fe9348bda250f8e804f26abb43e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.2 MB (562234162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d15abcb1eddfb6fb55b91a48996b9df904445cb8452ff8a39e0137cbb81b376`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:20 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:20 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:39 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:42 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:42 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:42 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:42 GMT
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
	-	`sha256:6c79339b9b2b6885c214417e76cbd4c9c8b40138f738d676d875e42621f2a386`  
		Last Modified: Wed, 05 Jul 2023 05:01:38 GMT  
		Size: 468.9 MB (468887312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb254725b1b44ca37f9c4dd1ef91a6671f1fb93c6dae8e868c4b1a52bca0c39`  
		Last Modified: Wed, 05 Jul 2023 05:01:21 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:10.1.0-enterprise`

```console
$ docker pull sonarqube@sha256:6c042122eead371f181fff91a777dcc48bccf3351d7bfbacd4a4c548ac20cc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:10.1.0-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:35fe3b6a46135100a3dc72b3e7ea18fe5d5b3959e34ef0d25796d95c234d3a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.7 MB (582679450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3e99d5970b424fb459824593f5e9f16b0f3666d1e8a888a933e18ce56747a`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:30 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:30 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:50 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:51 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:51 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:52 GMT
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
	-	`sha256:97dc6fffa26b5098e6e70351cb4bb0637d2c949686e15f77513650b39d46ea47`  
		Last Modified: Wed, 05 Jul 2023 12:28:21 GMT  
		Size: 488.2 MB (488200311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a2fd8aed8319f291cb298c7bcd000cad1f32f21ec7b0a61a800592d03077bf`  
		Last Modified: Wed, 05 Jul 2023 12:28:01 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:10.1.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:558f2d23ade2903aaccd3be190b4466c5ad7430e7538e5564f78eaac864a5eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.5 MB (581528720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9055674352aaa3245776b65d1d235b6d5ca440c63e6d47e1c3f953d2a6c39114`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:48 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:56:24 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:56:28 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:56:28 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:56:28 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:56:28 GMT
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
	-	`sha256:09af0d1bb681e0a7877489253a8c5c13161b5c43f87a36dd802b65ea640667d4`  
		Last Modified: Wed, 05 Jul 2023 05:02:08 GMT  
		Size: 488.2 MB (488181869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc199f6b625587da3609df62174b04bc0ff8b7315b7b0e1333baa4afd83e7eb`  
		Last Modified: Wed, 05 Jul 2023 05:01:51 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9-community`

```console
$ docker pull sonarqube@sha256:34f37d08af7988c0d2cfa5732f37209b03d8607e7fa6869f4f08635ae6946e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:954a02ba94a6301ff5a5057c16086ce75acc5b1654b3705ad9289154a87a6521
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395632092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f8f50567764add805039625e65e1292e2420e168b699285ae862466ff80997`
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
# Wed, 05 Jul 2023 12:19:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:19:36 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:19:55 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:19:55 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:19:55 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:19:55 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:19:55 GMT
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
	-	`sha256:881e5283bff97ce629ff456cae25a0dba4c83469afd886d03be27b4cca44e531`  
		Last Modified: Wed, 05 Jul 2023 12:24:37 GMT  
		Size: 301.2 MB (301152954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ccfd8bfc736257357a0ce3f5dc4e40cc3345b926ddb15728dc4edaed97c55b`  
		Last Modified: Wed, 05 Jul 2023 12:24:23 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:96714f0ec3879ba8deb401dfce80ea35fe7cd19f1ea6bbf26206d3bc41b06a1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.5 MB (394481854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbf31b36e0ab4bc5bf09444624b9524a82f5131756e223957cd2d2445846ea0`
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
# Wed, 05 Jul 2023 04:52:10 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:52:29 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:52:31 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:52:31 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:52:31 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:52:31 GMT
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
	-	`sha256:e0a862d6b45833cb8661dccf30af4c74ec96aaa89814276d52f7cd0db6a4a195`  
		Last Modified: Wed, 05 Jul 2023 04:58:44 GMT  
		Size: 301.1 MB (301135003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45044947eb570d0b5edb0fd16dd331157c60d6feef3e642d93ec8cfd61171579`  
		Last Modified: Wed, 05 Jul 2023 04:58:32 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9-datacenter-app`

```console
$ docker pull sonarqube@sha256:40373a7e11eaee74a071086dd73119211ae778617fb7bd1c55328cfb6012eb22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:971b9ee133d8298e10df6dcb639a6e4ac103da2067818e385fbba87652d07518
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df225846aff5a406edebd256f2f5a8f55925d9a1ab09a67b32f2ed4c34467960`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:49 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:12 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:13 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:13 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:13 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:13 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:13 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1c93d4aeb74e47ebd903bfd8f0f56aed570ea3da45e0103502e24fdec5cbfb36`  
		Last Modified: Wed, 05 Jul 2023 12:26:10 GMT  
		Size: 438.9 MB (438851096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b732e70c229fe7ec91627944f40cdc012d0b02a40b36078e7c73714d4b2bde`  
		Last Modified: Wed, 05 Jul 2023 12:25:52 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dd44e3e2e501f2257bfd7ff25cb166a0a82646b41271623af1fc5d75aa28a2ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2857358ce3ee88c9d56fe9efffcb2e52b3366f7764e94d2cf78467a34021c015`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:41 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:20 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:23 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:24 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:24 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:24 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:24 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:26ccadbd710dbd273041a9113b85a7f344788f3b3769a2a0292eeeb8280c3787`  
		Last Modified: Wed, 05 Jul 2023 05:00:07 GMT  
		Size: 438.8 MB (438839299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d1863781999f78b2f2c5f5deec00550ff93ba0bf713328e74b0c009e19726d`  
		Last Modified: Wed, 05 Jul 2023 04:59:51 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9-datacenter-search`

```console
$ docker pull sonarqube@sha256:a4bf12590eb27b10fcdcc1aef833bcb412a7b8e35a0fbc631dadf0d35485931f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:a02d21c62773e17d2a763858d6fac16e92f95496bda86f7227a11f5f50109ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dde400c8c295fe04397338f3fa84872f71411acc380379fc3620a21a29fd3a2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:21:17 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:37 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:38 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:38 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:38 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:38 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:38 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:7aa08cde7d1ad6ebb5eb06ce4da65c81367ef840bf6a93a1bc48c8fd8b5521f3`  
		Last Modified: Wed, 05 Jul 2023 12:26:41 GMT  
		Size: 438.9 MB (438851010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a616ebb74cd6de753e6d804d59acd575cb427fe99f84014d59925473143053db`  
		Last Modified: Wed, 05 Jul 2023 12:26:23 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:b444c4d8a950e45e426cd00e2e558383e527b0be7178a2da62df936f60176186
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454bac5a56d2a06bf2ca7380c574413740dc473afce2b967e7d437aa67d39896`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:54:29 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:48 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:51 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:52 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:52 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:52 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:52 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:b8e6a965ac6e161ca24e2bb7d25d6198acced8db455f2eada396fa373bcf493f`  
		Last Modified: Wed, 05 Jul 2023 05:00:38 GMT  
		Size: 438.8 MB (438839251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b501b4020e4d90a9108e4be36880d28be5206574ed4bf2d4b0c8cdec057a2a83`  
		Last Modified: Wed, 05 Jul 2023 05:00:23 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `sonarqube:9-enterprise`

```console
$ docker pull sonarqube@sha256:6fff5e2a05bb609474d7fd074caf8e119c9c312ac9597bb9ed16d022324f09c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:57ff04c94c9d2caf9097f50ca8c3b185fc65610bcf4620900c48bad4229ab204
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.2 MB (509170570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f748885095e8b38023aa07536383e5d782de31fb5b3c4e4f8b43f63846a31be8`
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
# Wed, 05 Jul 2023 12:20:24 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:24 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:20:43 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:20:44 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:20:44 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:20:44 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:20:44 GMT
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
	-	`sha256:90af63c01db9af4e7ec43dafb96f7819e6736e82e5a79d00ff356aaf6bc55082`  
		Last Modified: Wed, 05 Jul 2023 12:25:38 GMT  
		Size: 414.7 MB (414691432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c665896087acde5dd32e04550e5e460bd7744d00650322f78258314158aeda3`  
		Last Modified: Wed, 05 Jul 2023 12:25:20 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:812f24b13806d481624bb2addc96fe544c4b335e3a76670fa2a882fa446eabd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **508.0 MB (508017885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4366466172eea87b3cd444402105f8579d12a4811fb857fc1ee25d68884a74d9`
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
# Wed, 05 Jul 2023 04:53:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:13 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:53:32 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:53:35 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:53:35 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:53:35 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:53:35 GMT
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
	-	`sha256:5a903515327de7a4e84b4e73937f2f2bed28c92ada7fbb52c216b3b0c9ace9d7`  
		Last Modified: Wed, 05 Jul 2023 04:59:39 GMT  
		Size: 414.7 MB (414671034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37c5d3013dc65ee7eef6d7b7442a8751a28e60815eb671ce8d9678debdc55a8`  
		Last Modified: Wed, 05 Jul 2023 04:59:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9-community`

```console
$ docker pull sonarqube@sha256:34f37d08af7988c0d2cfa5732f37209b03d8607e7fa6869f4f08635ae6946e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:954a02ba94a6301ff5a5057c16086ce75acc5b1654b3705ad9289154a87a6521
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395632092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f8f50567764add805039625e65e1292e2420e168b699285ae862466ff80997`
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
# Wed, 05 Jul 2023 12:19:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:19:36 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:19:55 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:19:55 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:19:55 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:19:55 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:19:55 GMT
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
	-	`sha256:881e5283bff97ce629ff456cae25a0dba4c83469afd886d03be27b4cca44e531`  
		Last Modified: Wed, 05 Jul 2023 12:24:37 GMT  
		Size: 301.2 MB (301152954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ccfd8bfc736257357a0ce3f5dc4e40cc3345b926ddb15728dc4edaed97c55b`  
		Last Modified: Wed, 05 Jul 2023 12:24:23 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:96714f0ec3879ba8deb401dfce80ea35fe7cd19f1ea6bbf26206d3bc41b06a1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.5 MB (394481854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbf31b36e0ab4bc5bf09444624b9524a82f5131756e223957cd2d2445846ea0`
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
# Wed, 05 Jul 2023 04:52:10 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:52:29 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:52:31 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:52:31 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:52:31 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:52:31 GMT
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
	-	`sha256:e0a862d6b45833cb8661dccf30af4c74ec96aaa89814276d52f7cd0db6a4a195`  
		Last Modified: Wed, 05 Jul 2023 04:58:44 GMT  
		Size: 301.1 MB (301135003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45044947eb570d0b5edb0fd16dd331157c60d6feef3e642d93ec8cfd61171579`  
		Last Modified: Wed, 05 Jul 2023 04:58:32 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9-datacenter-app`

```console
$ docker pull sonarqube@sha256:40373a7e11eaee74a071086dd73119211ae778617fb7bd1c55328cfb6012eb22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:971b9ee133d8298e10df6dcb639a6e4ac103da2067818e385fbba87652d07518
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df225846aff5a406edebd256f2f5a8f55925d9a1ab09a67b32f2ed4c34467960`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:49 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:12 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:13 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:13 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:13 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:13 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:13 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1c93d4aeb74e47ebd903bfd8f0f56aed570ea3da45e0103502e24fdec5cbfb36`  
		Last Modified: Wed, 05 Jul 2023 12:26:10 GMT  
		Size: 438.9 MB (438851096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b732e70c229fe7ec91627944f40cdc012d0b02a40b36078e7c73714d4b2bde`  
		Last Modified: Wed, 05 Jul 2023 12:25:52 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dd44e3e2e501f2257bfd7ff25cb166a0a82646b41271623af1fc5d75aa28a2ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2857358ce3ee88c9d56fe9efffcb2e52b3366f7764e94d2cf78467a34021c015`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:41 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:20 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:23 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:24 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:24 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:24 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:24 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:26ccadbd710dbd273041a9113b85a7f344788f3b3769a2a0292eeeb8280c3787`  
		Last Modified: Wed, 05 Jul 2023 05:00:07 GMT  
		Size: 438.8 MB (438839299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d1863781999f78b2f2c5f5deec00550ff93ba0bf713328e74b0c009e19726d`  
		Last Modified: Wed, 05 Jul 2023 04:59:51 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9-datacenter-search`

```console
$ docker pull sonarqube@sha256:a4bf12590eb27b10fcdcc1aef833bcb412a7b8e35a0fbc631dadf0d35485931f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:a02d21c62773e17d2a763858d6fac16e92f95496bda86f7227a11f5f50109ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dde400c8c295fe04397338f3fa84872f71411acc380379fc3620a21a29fd3a2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:21:17 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:37 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:38 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:38 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:38 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:38 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:38 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:7aa08cde7d1ad6ebb5eb06ce4da65c81367ef840bf6a93a1bc48c8fd8b5521f3`  
		Last Modified: Wed, 05 Jul 2023 12:26:41 GMT  
		Size: 438.9 MB (438851010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a616ebb74cd6de753e6d804d59acd575cb427fe99f84014d59925473143053db`  
		Last Modified: Wed, 05 Jul 2023 12:26:23 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:b444c4d8a950e45e426cd00e2e558383e527b0be7178a2da62df936f60176186
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454bac5a56d2a06bf2ca7380c574413740dc473afce2b967e7d437aa67d39896`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:54:29 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:48 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:51 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:52 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:52 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:52 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:52 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:b8e6a965ac6e161ca24e2bb7d25d6198acced8db455f2eada396fa373bcf493f`  
		Last Modified: Wed, 05 Jul 2023 05:00:38 GMT  
		Size: 438.8 MB (438839251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b501b4020e4d90a9108e4be36880d28be5206574ed4bf2d4b0c8cdec057a2a83`  
		Last Modified: Wed, 05 Jul 2023 05:00:23 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9-developer`

```console
$ docker pull sonarqube@sha256:d231773f02bf99229353792408e96ad75c537d0f93ce66f67dcd61dc9e2e40d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9-developer` - linux; amd64

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

### `sonarqube:9.9-developer` - linux; arm64 variant v8

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

## `sonarqube:9.9-enterprise`

```console
$ docker pull sonarqube@sha256:6fff5e2a05bb609474d7fd074caf8e119c9c312ac9597bb9ed16d022324f09c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:57ff04c94c9d2caf9097f50ca8c3b185fc65610bcf4620900c48bad4229ab204
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.2 MB (509170570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f748885095e8b38023aa07536383e5d782de31fb5b3c4e4f8b43f63846a31be8`
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
# Wed, 05 Jul 2023 12:20:24 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:24 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:20:43 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:20:44 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:20:44 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:20:44 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:20:44 GMT
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
	-	`sha256:90af63c01db9af4e7ec43dafb96f7819e6736e82e5a79d00ff356aaf6bc55082`  
		Last Modified: Wed, 05 Jul 2023 12:25:38 GMT  
		Size: 414.7 MB (414691432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c665896087acde5dd32e04550e5e460bd7744d00650322f78258314158aeda3`  
		Last Modified: Wed, 05 Jul 2023 12:25:20 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:812f24b13806d481624bb2addc96fe544c4b335e3a76670fa2a882fa446eabd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **508.0 MB (508017885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4366466172eea87b3cd444402105f8579d12a4811fb857fc1ee25d68884a74d9`
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
# Wed, 05 Jul 2023 04:53:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:13 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:53:32 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:53:35 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:53:35 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:53:35 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:53:35 GMT
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
	-	`sha256:5a903515327de7a4e84b4e73937f2f2bed28c92ada7fbb52c216b3b0c9ace9d7`  
		Last Modified: Wed, 05 Jul 2023 04:59:39 GMT  
		Size: 414.7 MB (414671034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37c5d3013dc65ee7eef6d7b7442a8751a28e60815eb671ce8d9678debdc55a8`  
		Last Modified: Wed, 05 Jul 2023 04:59:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9.1-community`

```console
$ docker pull sonarqube@sha256:34f37d08af7988c0d2cfa5732f37209b03d8607e7fa6869f4f08635ae6946e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9.1-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:954a02ba94a6301ff5a5057c16086ce75acc5b1654b3705ad9289154a87a6521
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395632092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f8f50567764add805039625e65e1292e2420e168b699285ae862466ff80997`
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
# Wed, 05 Jul 2023 12:19:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:19:36 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:19:55 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:19:55 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:19:55 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:19:55 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:19:55 GMT
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
	-	`sha256:881e5283bff97ce629ff456cae25a0dba4c83469afd886d03be27b4cca44e531`  
		Last Modified: Wed, 05 Jul 2023 12:24:37 GMT  
		Size: 301.2 MB (301152954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ccfd8bfc736257357a0ce3f5dc4e40cc3345b926ddb15728dc4edaed97c55b`  
		Last Modified: Wed, 05 Jul 2023 12:24:23 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9.1-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:96714f0ec3879ba8deb401dfce80ea35fe7cd19f1ea6bbf26206d3bc41b06a1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.5 MB (394481854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbf31b36e0ab4bc5bf09444624b9524a82f5131756e223957cd2d2445846ea0`
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
# Wed, 05 Jul 2023 04:52:10 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:52:29 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:52:31 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:52:31 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:52:31 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:52:31 GMT
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
	-	`sha256:e0a862d6b45833cb8661dccf30af4c74ec96aaa89814276d52f7cd0db6a4a195`  
		Last Modified: Wed, 05 Jul 2023 04:58:44 GMT  
		Size: 301.1 MB (301135003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45044947eb570d0b5edb0fd16dd331157c60d6feef3e642d93ec8cfd61171579`  
		Last Modified: Wed, 05 Jul 2023 04:58:32 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9.1-datacenter-app`

```console
$ docker pull sonarqube@sha256:40373a7e11eaee74a071086dd73119211ae778617fb7bd1c55328cfb6012eb22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9.1-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:971b9ee133d8298e10df6dcb639a6e4ac103da2067818e385fbba87652d07518
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df225846aff5a406edebd256f2f5a8f55925d9a1ab09a67b32f2ed4c34467960`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:49 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:12 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:13 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:13 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:13 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:13 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:13 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1c93d4aeb74e47ebd903bfd8f0f56aed570ea3da45e0103502e24fdec5cbfb36`  
		Last Modified: Wed, 05 Jul 2023 12:26:10 GMT  
		Size: 438.9 MB (438851096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b732e70c229fe7ec91627944f40cdc012d0b02a40b36078e7c73714d4b2bde`  
		Last Modified: Wed, 05 Jul 2023 12:25:52 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9.1-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dd44e3e2e501f2257bfd7ff25cb166a0a82646b41271623af1fc5d75aa28a2ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2857358ce3ee88c9d56fe9efffcb2e52b3366f7764e94d2cf78467a34021c015`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:41 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:20 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:23 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:24 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:24 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:24 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:24 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:26ccadbd710dbd273041a9113b85a7f344788f3b3769a2a0292eeeb8280c3787`  
		Last Modified: Wed, 05 Jul 2023 05:00:07 GMT  
		Size: 438.8 MB (438839299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d1863781999f78b2f2c5f5deec00550ff93ba0bf713328e74b0c009e19726d`  
		Last Modified: Wed, 05 Jul 2023 04:59:51 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9.1-datacenter-search`

```console
$ docker pull sonarqube@sha256:a4bf12590eb27b10fcdcc1aef833bcb412a7b8e35a0fbc631dadf0d35485931f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9.1-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:a02d21c62773e17d2a763858d6fac16e92f95496bda86f7227a11f5f50109ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dde400c8c295fe04397338f3fa84872f71411acc380379fc3620a21a29fd3a2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:21:17 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:37 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:38 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:38 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:38 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:38 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:38 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:7aa08cde7d1ad6ebb5eb06ce4da65c81367ef840bf6a93a1bc48c8fd8b5521f3`  
		Last Modified: Wed, 05 Jul 2023 12:26:41 GMT  
		Size: 438.9 MB (438851010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a616ebb74cd6de753e6d804d59acd575cb427fe99f84014d59925473143053db`  
		Last Modified: Wed, 05 Jul 2023 12:26:23 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9.1-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:b444c4d8a950e45e426cd00e2e558383e527b0be7178a2da62df936f60176186
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454bac5a56d2a06bf2ca7380c574413740dc473afce2b967e7d437aa67d39896`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:54:29 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:48 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:51 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:52 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:52 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:52 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:52 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:b8e6a965ac6e161ca24e2bb7d25d6198acced8db455f2eada396fa373bcf493f`  
		Last Modified: Wed, 05 Jul 2023 05:00:38 GMT  
		Size: 438.8 MB (438839251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b501b4020e4d90a9108e4be36880d28be5206574ed4bf2d4b0c8cdec057a2a83`  
		Last Modified: Wed, 05 Jul 2023 05:00:23 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:9.9.1-developer`

```console
$ docker pull sonarqube@sha256:d231773f02bf99229353792408e96ad75c537d0f93ce66f67dcd61dc9e2e40d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9.1-developer` - linux; amd64

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

### `sonarqube:9.9.1-developer` - linux; arm64 variant v8

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

## `sonarqube:9.9.1-enterprise`

```console
$ docker pull sonarqube@sha256:6fff5e2a05bb609474d7fd074caf8e119c9c312ac9597bb9ed16d022324f09c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:9.9.1-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:57ff04c94c9d2caf9097f50ca8c3b185fc65610bcf4620900c48bad4229ab204
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.2 MB (509170570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f748885095e8b38023aa07536383e5d782de31fb5b3c4e4f8b43f63846a31be8`
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
# Wed, 05 Jul 2023 12:20:24 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:24 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:20:43 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:20:44 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:20:44 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:20:44 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:20:44 GMT
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
	-	`sha256:90af63c01db9af4e7ec43dafb96f7819e6736e82e5a79d00ff356aaf6bc55082`  
		Last Modified: Wed, 05 Jul 2023 12:25:38 GMT  
		Size: 414.7 MB (414691432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c665896087acde5dd32e04550e5e460bd7744d00650322f78258314158aeda3`  
		Last Modified: Wed, 05 Jul 2023 12:25:20 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:9.9.1-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:812f24b13806d481624bb2addc96fe544c4b335e3a76670fa2a882fa446eabd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **508.0 MB (508017885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4366466172eea87b3cd444402105f8579d12a4811fb857fc1ee25d68884a74d9`
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
# Wed, 05 Jul 2023 04:53:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:13 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:53:32 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:53:35 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:53:35 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:53:35 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:53:35 GMT
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
	-	`sha256:5a903515327de7a4e84b4e73937f2f2bed28c92ada7fbb52c216b3b0c9ace9d7`  
		Last Modified: Wed, 05 Jul 2023 04:59:39 GMT  
		Size: 414.7 MB (414671034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37c5d3013dc65ee7eef6d7b7442a8751a28e60815eb671ce8d9678debdc55a8`  
		Last Modified: Wed, 05 Jul 2023 04:59:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:community`

```console
$ docker pull sonarqube@sha256:b0e9f03c5c1b9faf2c4cc3bbd81ef90d9df8876e9b40271881a6168774374c6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:community` - linux; amd64

```console
$ docker pull sonarqube@sha256:0f225682c2db92dd38514bddbed0bf2240a09386686d4462752dce91da594eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **468.4 MB (468359493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907b1b7b82bee77ada1c7170a6f72b871c806fc1a0e97d8e77490b7121c989e4`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:21:41 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:21:59 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:00 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:00 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:00 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:00 GMT
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
	-	`sha256:394329c8ee57507abde6133e4be41035dc28322b8d5784283c5c265bae0c8bee`  
		Last Modified: Wed, 05 Jul 2023 12:27:11 GMT  
		Size: 373.9 MB (373880354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c43f2deaf333887421a0851e818b61bfdde26ce80e2e1a4ab12ba7b0e45e7f`  
		Last Modified: Wed, 05 Jul 2023 12:26:55 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:89e3f27f2cc0c79aceb8c9e5f6e468cecffe3f90fe7eb7a3d599673fbd8681ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467198578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294c1b266c52c9dc89ba5c29465f3acf2c071526cbb311a6f88f2f957283ea56`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:54:57 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:15 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:18 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:18 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:18 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:18 GMT
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
	-	`sha256:3d6b64d2c7bbcaefb52364635d1548c284e9117ed6efbd12505e2a237f543f5d`  
		Last Modified: Wed, 05 Jul 2023 05:01:06 GMT  
		Size: 373.9 MB (373851726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8879d10617e8a246b0d1b696480ef4b420eb9025f14e5d811a11a7d3aa4fd`  
		Last Modified: Wed, 05 Jul 2023 05:00:52 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:datacenter-app`

```console
$ docker pull sonarqube@sha256:6e618f16f4e44f4dc893fb6787bd36a3aae6f16e9481fa7a7dc0a9242e52f1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:e4bd05d466fbd0b9b66c11e1990cf8c28169e8e38e595f50144915a1c9d1d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab37611fc601ab5f15c2eeb8de910e5aeb7c972d45437d62ece416701bd836a`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:58 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:19 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:20 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:20 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:20 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:20 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:21 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:21 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:21 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1a19a5a15e046b51dba9c274327dd2d4a6d061e6502370af23e3e199ca2981d4`  
		Last Modified: Wed, 05 Jul 2023 12:28:56 GMT  
		Size: 489.9 MB (489892103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499fdd0a44f41578c3f19fcfda431fcaf7ff5de1a51b0f22c978fb27139323f9`  
		Last Modified: Wed, 05 Jul 2023 12:28:35 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:fa566713c02911b39b4cbd5515e420aedcbd322cddee39e7e9cc7ebad9960e6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e66559188e80a0798a8f37b45c4313bd6d602beee0d53be08a4508467a7f96f`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:56:36 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:12 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:16 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:16 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:16 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:16 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:16 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:16 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:401cd866db1db244a28a6ea3dca1eb3552c1fe6bc03add294ccc23a7d3862ca9`  
		Last Modified: Wed, 05 Jul 2023 05:02:38 GMT  
		Size: 489.9 MB (489883219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b386629d530bc4be285e300df11a14a3a51b828e566f85566d0fe1ee39dfaa1`  
		Last Modified: Wed, 05 Jul 2023 05:02:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:datacenter-search`

```console
$ docker pull sonarqube@sha256:960f362615b5eff3d5ab194a547bc2a826d21fd68c6de5a0fade1e97883767e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:d1c1e4561863f74ce6a50bd154017f4cf41567f628e2b26838ad1ff4d4c70016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.4 MB (584371530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73745fb21b7da208e5feb707787ff0a09aa1bcdac9fc940416c58a22a873b0fd`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:58 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:23:27 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:23:48 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:23:50 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:23:50 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:23:50 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:23:50 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:23:50 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:23:50 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:cd46c70cb09fa784a36370697038d617deb109c9f68de0b5e5c3a90b0d94c026`  
		Last Modified: Wed, 05 Jul 2023 12:29:29 GMT  
		Size: 489.9 MB (489892014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10558e306e9893095b53fd9dc8f767b7ba0610457756aeeb15d7167a78368dde`  
		Last Modified: Wed, 05 Jul 2023 12:29:08 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dac3679f797bfa190f5c37b028d202e74724ea79adbd6391e3e8d3233f1b6ba8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583230413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:602b8be520c0e71f321f7bb48123afbc67426e41d9022f8afe1ed762f12eb6f2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:56:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:57:24 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:57:53 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:57:57 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:57:57 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:57:57 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:57:57 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:57:57 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:57:57 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:75115b4064ce43511001eb98c1d542db9257cb93e39dc932a702078f33220691`  
		Last Modified: Wed, 05 Jul 2023 05:03:09 GMT  
		Size: 489.9 MB (489883187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8375ad97f4ec6161b377ff8c8af6a2d479e86e43a221aa5b27eb7ddbb44272`  
		Last Modified: Wed, 05 Jul 2023 05:02:51 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:developer`

```console
$ docker pull sonarqube@sha256:04c0882d01c2ccf9e4eb7c43c9734987dca083599cb9926c403c41e0ab9ec61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:04d8ba491263a8391721448ebe847ac67ed0b2f4106f7952d66e10d9fee3186d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.4 MB (563384649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef08e724cfe7dfc2b2b3142a72fc7372c68466bf49b37a2f5a583a952efe504c`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:05 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:06 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:25 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:26 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:26 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:26 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:27 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:27 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:27 GMT
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
	-	`sha256:8066a59c1bbd3583352b0b54ee0b323e7839f03fbfe4e24c3c69ce7d282a095a`  
		Last Modified: Wed, 05 Jul 2023 12:27:48 GMT  
		Size: 468.9 MB (468905509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b140a90a298d12f2681656f58b556cb7e6ca6529c259ad1882dc04c53be712`  
		Last Modified: Wed, 05 Jul 2023 12:27:25 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:developer` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:63a2db596e0a79fdc086a54af2c7d1999749fe9348bda250f8e804f26abb43e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.2 MB (562234162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d15abcb1eddfb6fb55b91a48996b9df904445cb8452ff8a39e0137cbb81b376`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:20 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:20 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:39 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:42 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:42 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:42 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:42 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:42 GMT
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
	-	`sha256:6c79339b9b2b6885c214417e76cbd4c9c8b40138f738d676d875e42621f2a386`  
		Last Modified: Wed, 05 Jul 2023 05:01:38 GMT  
		Size: 468.9 MB (468887312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb254725b1b44ca37f9c4dd1ef91a6671f1fb93c6dae8e868c4b1a52bca0c39`  
		Last Modified: Wed, 05 Jul 2023 05:01:21 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:enterprise`

```console
$ docker pull sonarqube@sha256:6c042122eead371f181fff91a777dcc48bccf3351d7bfbacd4a4c548ac20cc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:35fe3b6a46135100a3dc72b3e7ea18fe5d5b3959e34ef0d25796d95c234d3a35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.7 MB (582679450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3e99d5970b424fb459824593f5e9f16b0f3666d1e8a888a933e18ce56747a`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:22:30 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:22:30 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:22:50 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:51 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:51 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:51 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:52 GMT
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
	-	`sha256:97dc6fffa26b5098e6e70351cb4bb0637d2c949686e15f77513650b39d46ea47`  
		Last Modified: Wed, 05 Jul 2023 12:28:21 GMT  
		Size: 488.2 MB (488200311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a2fd8aed8319f291cb298c7bcd000cad1f32f21ec7b0a61a800592d03077bf`  
		Last Modified: Wed, 05 Jul 2023 12:28:01 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:558f2d23ade2903aaccd3be190b4466c5ad7430e7538e5564f78eaac864a5eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.5 MB (581528720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9055674352aaa3245776b65d1d235b6d5ca440c63e6d47e1c3f953d2a6c39114`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:55:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:55:48 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:56:24 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:56:28 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:56:28 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:56:28 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:56:28 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:56:28 GMT
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
	-	`sha256:09af0d1bb681e0a7877489253a8c5c13161b5c43f87a36dd802b65ea640667d4`  
		Last Modified: Wed, 05 Jul 2023 05:02:08 GMT  
		Size: 488.2 MB (488181869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc199f6b625587da3609df62174b04bc0ff8b7315b7b0e1333baa4afd83e7eb`  
		Last Modified: Wed, 05 Jul 2023 05:01:51 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:latest`

```console
$ docker pull sonarqube@sha256:b0e9f03c5c1b9faf2c4cc3bbd81ef90d9df8876e9b40271881a6168774374c6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:latest` - linux; amd64

```console
$ docker pull sonarqube@sha256:0f225682c2db92dd38514bddbed0bf2240a09386686d4462752dce91da594eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **468.4 MB (468359493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907b1b7b82bee77ada1c7170a6f72b871c806fc1a0e97d8e77490b7121c989e4`
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
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 12:21:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 12:21:41 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:21:59 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:22:00 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:22:00 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:22:00 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:22:00 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:22:00 GMT
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
	-	`sha256:394329c8ee57507abde6133e4be41035dc28322b8d5784283c5c265bae0c8bee`  
		Last Modified: Wed, 05 Jul 2023 12:27:11 GMT  
		Size: 373.9 MB (373880354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c43f2deaf333887421a0851e818b61bfdde26ce80e2e1a4ab12ba7b0e45e7f`  
		Last Modified: Wed, 05 Jul 2023 12:26:55 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:latest` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:89e3f27f2cc0c79aceb8c9e5f6e468cecffe3f90fe7eb7a3d599673fbd8681ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467198578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294c1b266c52c9dc89ba5c29465f3acf2c071526cbb311a6f88f2f957283ea56`
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
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_VERSION=10.1.0.73491
# Wed, 05 Jul 2023 04:54:57 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
# Wed, 05 Jul 2023 04:54:57 GMT
ENV DOCKER_RUNNING=true JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=10.1.0.73491 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:55:15 GMT
# ARGS: SONARQUBE_VERSION=10.1.0.73491 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.1.0.73491.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:55:18 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:55:18 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:55:18 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:55:18 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:55:18 GMT
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
	-	`sha256:3d6b64d2c7bbcaefb52364635d1548c284e9117ed6efbd12505e2a237f543f5d`  
		Last Modified: Wed, 05 Jul 2023 05:01:06 GMT  
		Size: 373.9 MB (373851726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8879d10617e8a246b0d1b696480ef4b420eb9025f14e5d811a11a7d3aa4fd`  
		Last Modified: Wed, 05 Jul 2023 05:00:52 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts`

```console
$ docker pull sonarqube@sha256:34f37d08af7988c0d2cfa5732f37209b03d8607e7fa6869f4f08635ae6946e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:lts` - linux; amd64

```console
$ docker pull sonarqube@sha256:954a02ba94a6301ff5a5057c16086ce75acc5b1654b3705ad9289154a87a6521
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395632092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f8f50567764add805039625e65e1292e2420e168b699285ae862466ff80997`
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
# Wed, 05 Jul 2023 12:19:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:19:36 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:19:55 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:19:55 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:19:55 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:19:55 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:19:55 GMT
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
	-	`sha256:881e5283bff97ce629ff456cae25a0dba4c83469afd886d03be27b4cca44e531`  
		Last Modified: Wed, 05 Jul 2023 12:24:37 GMT  
		Size: 301.2 MB (301152954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ccfd8bfc736257357a0ce3f5dc4e40cc3345b926ddb15728dc4edaed97c55b`  
		Last Modified: Wed, 05 Jul 2023 12:24:23 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:lts` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:96714f0ec3879ba8deb401dfce80ea35fe7cd19f1ea6bbf26206d3bc41b06a1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.5 MB (394481854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbf31b36e0ab4bc5bf09444624b9524a82f5131756e223957cd2d2445846ea0`
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
# Wed, 05 Jul 2023 04:52:10 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:52:29 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:52:31 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:52:31 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:52:31 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:52:31 GMT
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
	-	`sha256:e0a862d6b45833cb8661dccf30af4c74ec96aaa89814276d52f7cd0db6a4a195`  
		Last Modified: Wed, 05 Jul 2023 04:58:44 GMT  
		Size: 301.1 MB (301135003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45044947eb570d0b5edb0fd16dd331157c60d6feef3e642d93ec8cfd61171579`  
		Last Modified: Wed, 05 Jul 2023 04:58:32 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts-community`

```console
$ docker pull sonarqube@sha256:34f37d08af7988c0d2cfa5732f37209b03d8607e7fa6869f4f08635ae6946e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:lts-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:954a02ba94a6301ff5a5057c16086ce75acc5b1654b3705ad9289154a87a6521
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395632092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f8f50567764add805039625e65e1292e2420e168b699285ae862466ff80997`
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
# Wed, 05 Jul 2023 12:19:36 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:19:36 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:19:55 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:19:55 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:19:55 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:19:55 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:19:55 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:19:55 GMT
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
	-	`sha256:881e5283bff97ce629ff456cae25a0dba4c83469afd886d03be27b4cca44e531`  
		Last Modified: Wed, 05 Jul 2023 12:24:37 GMT  
		Size: 301.2 MB (301152954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ccfd8bfc736257357a0ce3f5dc4e40cc3345b926ddb15728dc4edaed97c55b`  
		Last Modified: Wed, 05 Jul 2023 12:24:23 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:lts-community` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:96714f0ec3879ba8deb401dfce80ea35fe7cd19f1ea6bbf26206d3bc41b06a1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.5 MB (394481854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbf31b36e0ab4bc5bf09444624b9524a82f5131756e223957cd2d2445846ea0`
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
# Wed, 05 Jul 2023 04:52:10 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:52:29 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:52:31 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:52:31 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:52:31 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:52:31 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:52:31 GMT
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
	-	`sha256:e0a862d6b45833cb8661dccf30af4c74ec96aaa89814276d52f7cd0db6a4a195`  
		Last Modified: Wed, 05 Jul 2023 04:58:44 GMT  
		Size: 301.1 MB (301135003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45044947eb570d0b5edb0fd16dd331157c60d6feef3e642d93ec8cfd61171579`  
		Last Modified: Wed, 05 Jul 2023 04:58:32 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts-datacenter-app`

```console
$ docker pull sonarqube@sha256:40373a7e11eaee74a071086dd73119211ae778617fb7bd1c55328cfb6012eb22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:lts-datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:971b9ee133d8298e10df6dcb639a6e4ac103da2067818e385fbba87652d07518
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df225846aff5a406edebd256f2f5a8f55925d9a1ab09a67b32f2ed4c34467960`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:49 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:12 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:13 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:13 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:13 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:13 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:13 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:13 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:1c93d4aeb74e47ebd903bfd8f0f56aed570ea3da45e0103502e24fdec5cbfb36`  
		Last Modified: Wed, 05 Jul 2023 12:26:10 GMT  
		Size: 438.9 MB (438851096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b732e70c229fe7ec91627944f40cdc012d0b02a40b36078e7c73714d4b2bde`  
		Last Modified: Wed, 05 Jul 2023 12:25:52 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:lts-datacenter-app` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:dd44e3e2e501f2257bfd7ff25cb166a0a82646b41271623af1fc5d75aa28a2ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2857358ce3ee88c9d56fe9efffcb2e52b3366f7764e94d2cf78467a34021c015`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:41 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:20 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:23 GMT
COPY multi:7b7719bed96cd17241806a1f2a9ebb6f7dbc11dd28a809f25f28515547af5f31 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:24 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:24 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:24 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:24 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:24 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:26ccadbd710dbd273041a9113b85a7f344788f3b3769a2a0292eeeb8280c3787`  
		Last Modified: Wed, 05 Jul 2023 05:00:07 GMT  
		Size: 438.8 MB (438839299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d1863781999f78b2f2c5f5deec00550ff93ba0bf713328e74b0c009e19726d`  
		Last Modified: Wed, 05 Jul 2023 04:59:51 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts-datacenter-search`

```console
$ docker pull sonarqube@sha256:a4bf12590eb27b10fcdcc1aef833bcb412a7b8e35a0fbc631dadf0d35485931f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:lts-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:a02d21c62773e17d2a763858d6fac16e92f95496bda86f7227a11f5f50109ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533330523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dde400c8c295fe04397338f3fa84872f71411acc380379fc3620a21a29fd3a2`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 12:20:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:21:17 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 12:21:37 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:21:38 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:21:38 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:21:38 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:21:38 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:21:38 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 12:21:38 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:7aa08cde7d1ad6ebb5eb06ce4da65c81367ef840bf6a93a1bc48c8fd8b5521f3`  
		Last Modified: Wed, 05 Jul 2023 12:26:41 GMT  
		Size: 438.9 MB (438851010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a616ebb74cd6de753e6d804d59acd575cb427fe99f84014d59925473143053db`  
		Last Modified: Wed, 05 Jul 2023 12:26:23 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:lts-datacenter-search` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:b444c4d8a950e45e426cd00e2e558383e527b0be7178a2da62df936f60176186
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.2 MB (532186477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454bac5a56d2a06bf2ca7380c574413740dc473afce2b967e7d437aa67d39896`
-	Entrypoint: `["\/opt\/sonarqube\/docker\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/docker\/sonar.sh"]`

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
# Wed, 05 Jul 2023 04:53:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:54:29 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Wed, 05 Jul 2023 04:54:48 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu iproute2;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:54:51 GMT
COPY multi:89fb11c026d59f7ff1da134f38f8b83061dfa7ae0312554196386d5f7168240c in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:54:51 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:54:51 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:54:52 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:54:52 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:54:52 GMT
ENTRYPOINT ["/opt/sonarqube/docker/run.sh"]
# Wed, 05 Jul 2023 04:54:52 GMT
CMD ["/opt/sonarqube/docker/sonar.sh"]
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
	-	`sha256:b8e6a965ac6e161ca24e2bb7d25d6198acced8db455f2eada396fa373bcf493f`  
		Last Modified: Wed, 05 Jul 2023 05:00:38 GMT  
		Size: 438.8 MB (438839251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b501b4020e4d90a9108e4be36880d28be5206574ed4bf2d4b0c8cdec057a2a83`  
		Last Modified: Wed, 05 Jul 2023 05:00:23 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts-developer`

```console
$ docker pull sonarqube@sha256:d231773f02bf99229353792408e96ad75c537d0f93ce66f67dcd61dc9e2e40d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:lts-developer` - linux; amd64

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

### `sonarqube:lts-developer` - linux; arm64 variant v8

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

## `sonarqube:lts-enterprise`

```console
$ docker pull sonarqube@sha256:6fff5e2a05bb609474d7fd074caf8e119c9c312ac9597bb9ed16d022324f09c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sonarqube:lts-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:57ff04c94c9d2caf9097f50ca8c3b185fc65610bcf4620900c48bad4229ab204
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.2 MB (509170570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f748885095e8b38023aa07536383e5d782de31fb5b3c4e4f8b43f63846a31be8`
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
# Wed, 05 Jul 2023 12:20:24 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 12:20:24 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 12:20:43 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 12:20:44 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 12:20:44 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 12:20:44 GMT
USER sonarqube
# Wed, 05 Jul 2023 12:20:44 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 12:20:44 GMT
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
	-	`sha256:90af63c01db9af4e7ec43dafb96f7819e6736e82e5a79d00ff356aaf6bc55082`  
		Last Modified: Wed, 05 Jul 2023 12:25:38 GMT  
		Size: 414.7 MB (414691432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c665896087acde5dd32e04550e5e460bd7744d00650322f78258314158aeda3`  
		Last Modified: Wed, 05 Jul 2023 12:25:20 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sonarqube:lts-enterprise` - linux; arm64 variant v8

```console
$ docker pull sonarqube@sha256:812f24b13806d481624bb2addc96fe544c4b335e3a76670fa2a882fa446eabd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **508.0 MB (508017885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4366466172eea87b3cd444402105f8579d12a4811fb857fc1ee25d68884a74d9`
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
# Wed, 05 Jul 2023 04:53:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
# Wed, 05 Jul 2023 04:53:13 GMT
ENV JAVA_HOME=/opt/java/openjdk SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.9.1.69595 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 05 Jul 2023 04:53:32 GMT
# ARGS: SONARQUBE_VERSION=9.9.1.69595 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-9.9.1.69595.zip
RUN set -eux;     groupadd --system --gid 1000 sonarqube;     useradd --system --uid 1000 --gid sonarqube sonarqube;     apt-get update;     apt-get install -y gnupg unzip curl bash fonts-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e hkps://keys.openpgp.org                             hkps://keyserver.ubuntu.com) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     ln -s "${SONARQUBE_HOME}/lib/sonar-application-${SONARQUBE_VERSION}.jar" "${SONARQUBE_HOME}/lib/sonarqube.jar";     chmod -R 555 ${SONARQUBE_HOME};     chmod -R ugo+wrX "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}";     apt-get remove -y gnupg unzip curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Jul 2023 04:53:35 GMT
COPY file:51aced1b78206886f6fbafaa2cd9132831e659d7d4073dffca35b43d1847a323 in /opt/sonarqube/docker/ 
# Wed, 05 Jul 2023 04:53:35 GMT
WORKDIR /opt/sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
EXPOSE 9000
# Wed, 05 Jul 2023 04:53:35 GMT
USER sonarqube
# Wed, 05 Jul 2023 04:53:35 GMT
STOPSIGNAL SIGINT
# Wed, 05 Jul 2023 04:53:35 GMT
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
	-	`sha256:5a903515327de7a4e84b4e73937f2f2bed28c92ada7fbb52c216b3b0c9ace9d7`  
		Last Modified: Wed, 05 Jul 2023 04:59:39 GMT  
		Size: 414.7 MB (414671034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37c5d3013dc65ee7eef6d7b7442a8751a28e60815eb671ce8d9678debdc55a8`  
		Last Modified: Wed, 05 Jul 2023 04:59:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
