## `open-liberty:kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:8c6d6aebe67f763f70cfc7302f42c31e6d3ad30668b1267dce065364933e2599
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:6936fbd7a1f4ee74fd5c0f3d1f17fa5e2fcc4d08ba57d3268353799067fe6e44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113776604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14d83aab361d95ae81f4aa8e3d8984b88a309f0b13517593ac3c49960af0ca77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:46:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:46:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 00:19:41 GMT
ENV JAVA_VERSION=jdk8u372-b07_openj9-0.38.0
# Thu, 01 Jun 2023 00:22:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='b0d830c47350de0b9d056d60f98b48d0452183bb640a03b316028e3c7d603162';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='30e9a4c4bd693128a6d3e9244495b1ffc0255af9eb6183247b7c03580337284c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ad0829fbd2473704e8103524882bc25625958b6f3038e80f8a99ab926e6b58a3';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='5a0e098267ea57c5088c2c9d2a6f6bf0f8f3e1ed6fd6f1ebf4a7a94e02352dc4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 01 Jun 2023 00:22:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 00:22:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 01 Jun 2023 00:22:46 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 01 Jun 2023 17:51:46 GMT
ARG LIBERTY_VERSION=23.0.0.4
# Thu, 01 Jun 2023 17:51:46 GMT
ARG LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6
# Thu, 01 Jun 2023 17:51:46 GMT
ARG LIBERTY_BUILD_LABEL=cl230420230418-0035
# Thu, 01 Jun 2023 17:51:46 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip
# Thu, 01 Jun 2023 17:51:46 GMT
ARG OPENJ9_SCC=true
# Thu, 01 Jun 2023 17:51:46 GMT
ARG VERBOSE=false
# Thu, 01 Jun 2023 17:51:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=23.0.0.4
# Thu, 01 Jun 2023 17:51:47 GMT
COPY dir:e798a2695af2fc0aba3a4a1978d332ada9c81458064239fbbb6f273596bed843 in /opt/ol/helpers 
# Thu, 01 Jun 2023 17:51:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 01 Jun 2023 17:51:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 01 Jun 2023 17:51:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 01 Jun 2023 17:51:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 01 Jun 2023 17:51:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 01 Jun 2023 17:51:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 01 Jun 2023 17:51:58 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 01 Jun 2023 17:51:58 GMT
USER 1001
# Thu, 01 Jun 2023 17:51:58 GMT
EXPOSE 9080 9443
# Thu, 01 Jun 2023 17:51:58 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 01 Jun 2023 17:51:58 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59060db11c04ba6b24aa769f7968a1ff7e5c4029ff838bb2a0c95f83a0c318c2`  
		Last Modified: Tue, 18 Apr 2023 01:54:10 GMT  
		Size: 16.0 MB (16002795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b9eb62747044a2f39ce6945fb53a45fb9763c79a32bc3cac3f23fb7434270`  
		Last Modified: Thu, 01 Jun 2023 00:36:07 GMT  
		Size: 50.3 MB (50259598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd87c37aba964d3a7a8d78206b11ae0fae6a03098788a3d03f103c72e43a611`  
		Last Modified: Thu, 01 Jun 2023 00:36:03 GMT  
		Size: 4.2 MB (4191607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044e0362a61df9e5d42f4758cd9a6903d9b2556b1d5c19e7274bf5c70d0c8edc`  
		Last Modified: Thu, 01 Jun 2023 18:03:19 GMT  
		Size: 8.2 KB (8223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42b0cbef15999eefdbdfae60dba96fb6b92af449a9764d4006503be48911607`  
		Last Modified: Thu, 01 Jun 2023 18:03:17 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f533801fccc41348e35406f4a72ebbff3224538429abb404c805ac75b88dc`  
		Last Modified: Thu, 01 Jun 2023 18:03:18 GMT  
		Size: 12.2 MB (12216582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a385374f94b243e4b1fdfdc739a69078cae66185be22e6f22658f92e621cd56`  
		Last Modified: Thu, 01 Jun 2023 18:03:17 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86047919834d0fd58215f647a56b66c08c3a28d3e825d9333fc109987868f14`  
		Last Modified: Thu, 01 Jun 2023 18:03:17 GMT  
		Size: 9.3 KB (9342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6b4aeb0dfb6cb2f45a9b424f80bda74562ea98a88aa5bd0b00dca6d6b1f38d`  
		Last Modified: Thu, 01 Jun 2023 18:03:18 GMT  
		Size: 2.5 MB (2508703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; arm64 variant v8

```console
$ docker pull open-liberty@sha256:7f48c80342baef7c0f4676bd70e1664dff5c1f7475ee393503477f03062a16e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110373886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf6166d165a97107b920b287a7320eecd21653f728cd8907181b9a3076eaffd`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:45:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:45:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:39:35 GMT
ENV JAVA_VERSION=jdk8u372-b07_openj9-0.38.0
# Wed, 31 May 2023 23:42:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='b0d830c47350de0b9d056d60f98b48d0452183bb640a03b316028e3c7d603162';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='30e9a4c4bd693128a6d3e9244495b1ffc0255af9eb6183247b7c03580337284c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ad0829fbd2473704e8103524882bc25625958b6f3038e80f8a99ab926e6b58a3';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='5a0e098267ea57c5088c2c9d2a6f6bf0f8f3e1ed6fd6f1ebf4a7a94e02352dc4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 31 May 2023 23:42:12 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 May 2023 23:42:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 31 May 2023 23:42:46 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 01 Jun 2023 00:17:41 GMT
ARG LIBERTY_VERSION=23.0.0.4
# Thu, 01 Jun 2023 00:17:41 GMT
ARG LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6
# Thu, 01 Jun 2023 00:17:41 GMT
ARG LIBERTY_BUILD_LABEL=cl230420230418-0035
# Thu, 01 Jun 2023 00:17:41 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip
# Thu, 01 Jun 2023 00:17:41 GMT
ARG OPENJ9_SCC=true
# Thu, 01 Jun 2023 00:17:41 GMT
ARG VERBOSE=false
# Thu, 01 Jun 2023 00:17:41 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=23.0.0.4
# Thu, 01 Jun 2023 00:17:41 GMT
COPY dir:e798a2695af2fc0aba3a4a1978d332ada9c81458064239fbbb6f273596bed843 in /opt/ol/helpers 
# Thu, 01 Jun 2023 00:17:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 01 Jun 2023 00:17:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 01 Jun 2023 00:17:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 01 Jun 2023 00:17:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 01 Jun 2023 00:17:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 01 Jun 2023 00:17:50 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 01 Jun 2023 00:17:51 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 01 Jun 2023 00:17:51 GMT
USER 1001
# Thu, 01 Jun 2023 00:17:51 GMT
EXPOSE 9080 9443
# Thu, 01 Jun 2023 00:17:51 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 01 Jun 2023 00:17:51 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7751d4fbf2062d96159da55aa2a9331cd03b66d2d7a5bae5db82dd2693de8cb5`  
		Last Modified: Tue, 18 Apr 2023 01:53:16 GMT  
		Size: 15.9 MB (15865841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176134bb2c3b98b9ed567d665e08b890bc2552e3f6915fdad89afcfd8af9335a`  
		Last Modified: Wed, 31 May 2023 23:55:29 GMT  
		Size: 48.4 MB (48420062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74660d0c92ff6a57d2818144ff5562989972079125fbcce3e6ef17586aace3e`  
		Last Modified: Wed, 31 May 2023 23:55:25 GMT  
		Size: 4.0 MB (4040292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756105e3ff03fb4f207a7c379a6398ee84c10853a6edc94503a7e61d49f3c6fc`  
		Last Modified: Thu, 01 Jun 2023 00:27:45 GMT  
		Size: 8.2 KB (8226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb04c3c563f5fee84ef32ce0dc9f5f283a7f3023975525c7a82859d0790b6f9`  
		Last Modified: Thu, 01 Jun 2023 00:27:44 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bfcfd655d709f97a3184340f76b7b0a9a6dccd6d9c4a774987462677e13202`  
		Last Modified: Thu, 01 Jun 2023 00:27:45 GMT  
		Size: 12.2 MB (12205798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf4cdfb5b0969b10b742a3c1f1200c5a3467a74fe405dfee5224588772831ca`  
		Last Modified: Thu, 01 Jun 2023 00:27:44 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95423b9e2d4c9dd7a1925d5d225c6519c7504e4188157ef8525b2fb23d58a9dd`  
		Last Modified: Thu, 01 Jun 2023 00:27:44 GMT  
		Size: 9.3 KB (9343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2781b3743a8f089b144d5f64feb2938ea06dd76771ce77df9a4ce58ffede8daf`  
		Last Modified: Thu, 01 Jun 2023 00:27:44 GMT  
		Size: 2.6 MB (2626741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:033f540fb405da36a36b6ccf11dc4a4774db5eee941a4676cc513f9469f4fa93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119580328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43dd2b876464e4f5ba88de2b25315be88b8f47392bf1f38a3d02de152b2b347b`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:24:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:25:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 00:16:41 GMT
ENV JAVA_VERSION=jdk8u372-b07_openj9-0.38.0
# Thu, 01 Jun 2023 00:19:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='b0d830c47350de0b9d056d60f98b48d0452183bb640a03b316028e3c7d603162';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='30e9a4c4bd693128a6d3e9244495b1ffc0255af9eb6183247b7c03580337284c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ad0829fbd2473704e8103524882bc25625958b6f3038e80f8a99ab926e6b58a3';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='5a0e098267ea57c5088c2c9d2a6f6bf0f8f3e1ed6fd6f1ebf4a7a94e02352dc4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 01 Jun 2023 00:19:22 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 00:19:24 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 01 Jun 2023 00:20:04 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 01 Jun 2023 02:25:14 GMT
ARG LIBERTY_VERSION=23.0.0.4
# Thu, 01 Jun 2023 02:25:15 GMT
ARG LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6
# Thu, 01 Jun 2023 02:25:16 GMT
ARG LIBERTY_BUILD_LABEL=cl230420230418-0035
# Thu, 01 Jun 2023 02:25:17 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip
# Thu, 01 Jun 2023 02:25:18 GMT
ARG OPENJ9_SCC=true
# Thu, 01 Jun 2023 02:25:18 GMT
ARG VERBOSE=false
# Thu, 01 Jun 2023 02:25:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=23.0.0.4
# Thu, 01 Jun 2023 02:25:19 GMT
COPY dir:e798a2695af2fc0aba3a4a1978d332ada9c81458064239fbbb6f273596bed843 in /opt/ol/helpers 
# Thu, 01 Jun 2023 02:25:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 01 Jun 2023 02:25:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 01 Jun 2023 02:25:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 01 Jun 2023 02:25:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 01 Jun 2023 02:25:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 01 Jun 2023 02:25:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 01 Jun 2023 02:25:49 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 01 Jun 2023 02:25:50 GMT
USER 1001
# Thu, 01 Jun 2023 02:25:51 GMT
EXPOSE 9080 9443
# Thu, 01 Jun 2023 02:25:51 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 01 Jun 2023 02:25:52 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a328f93092ceadb7a1b931cc278addf4dfae1321b9f8ced8d4ea73dc90facfb`  
		Last Modified: Tue, 18 Apr 2023 01:34:37 GMT  
		Size: 17.2 MB (17176898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed6cd86f3acf3fd82aad73cbe9152dc0edcf31cf12d66c35b3addb6d8aba01e`  
		Last Modified: Thu, 01 Jun 2023 00:32:08 GMT  
		Size: 50.8 MB (50758395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9efae1f790de2c12e2e59b9dafdf215ba4df54d8cd8ac34b05dad888974a534`  
		Last Modified: Thu, 01 Jun 2023 00:31:59 GMT  
		Size: 3.6 MB (3550910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9f3ff9041012cf3526625c9ef00b13ec055797395c6a48cc0225f7817572a9`  
		Last Modified: Thu, 01 Jun 2023 02:52:27 GMT  
		Size: 8.2 KB (8224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509428d4a29ff1ad925797028be9646d6e9c7be7b85012cffab1734dae9b719c`  
		Last Modified: Thu, 01 Jun 2023 02:52:25 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57997f1066c14ebd1e51469d97276290c465b418602fc172cfe68e0f835400bd`  
		Last Modified: Thu, 01 Jun 2023 02:52:27 GMT  
		Size: 12.2 MB (12237500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f6d1ad2cab97614edd79a256b2319a697fde3aa908f2705ee8310b4689293a`  
		Last Modified: Thu, 01 Jun 2023 02:52:25 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34547634d925854a91e9ba70e0b243921008c27954d0ec6e16990e4f9c286df`  
		Last Modified: Thu, 01 Jun 2023 02:52:25 GMT  
		Size: 9.4 KB (9370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3869cf01756a5c615f49ce13588d11e0da9472046c21dc3229bce116b488c83b`  
		Last Modified: Thu, 01 Jun 2023 02:52:26 GMT  
		Size: 2.5 MB (2536850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:0147cb9a9c300bce839090d58fdad9ab75493f9536ecf582934ce112135e75df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.0 MB (112007056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f41fe4106e162f65a017628c7c77aacbed12d606406bba8e8046a495c156ef48`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:20:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:20:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:43:01 GMT
ENV JAVA_VERSION=jdk8u372-b07_openj9-0.38.0
# Wed, 31 May 2023 23:44:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='b0d830c47350de0b9d056d60f98b48d0452183bb640a03b316028e3c7d603162';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='30e9a4c4bd693128a6d3e9244495b1ffc0255af9eb6183247b7c03580337284c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ad0829fbd2473704e8103524882bc25625958b6f3038e80f8a99ab926e6b58a3';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='5a0e098267ea57c5088c2c9d2a6f6bf0f8f3e1ed6fd6f1ebf4a7a94e02352dc4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u372-b07_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_8u372b07_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 31 May 2023 23:44:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 May 2023 23:44:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 31 May 2023 23:45:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 01 Jun 2023 01:29:22 GMT
ARG LIBERTY_VERSION=23.0.0.4
# Thu, 01 Jun 2023 01:29:22 GMT
ARG LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6
# Thu, 01 Jun 2023 01:29:22 GMT
ARG LIBERTY_BUILD_LABEL=cl230420230418-0035
# Thu, 01 Jun 2023 01:29:23 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip
# Thu, 01 Jun 2023 01:29:23 GMT
ARG OPENJ9_SCC=true
# Thu, 01 Jun 2023 01:29:23 GMT
ARG VERBOSE=false
# Thu, 01 Jun 2023 01:29:23 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=23.0.0.4
# Thu, 01 Jun 2023 01:29:23 GMT
COPY dir:e798a2695af2fc0aba3a4a1978d332ada9c81458064239fbbb6f273596bed843 in /opt/ol/helpers 
# Thu, 01 Jun 2023 01:29:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 01 Jun 2023 01:29:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 01 Jun 2023 01:29:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 01 Jun 2023 01:29:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 01 Jun 2023 01:29:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 01 Jun 2023 01:29:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230420230418-0035 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/23.0.0.4/openliberty-kernel-23.0.0.4.zip LIBERTY_SHA=e252710521c859f732769380db9b60e110119ed6 LIBERTY_VERSION=23.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 01 Jun 2023 01:29:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 01 Jun 2023 01:29:33 GMT
USER 1001
# Thu, 01 Jun 2023 01:29:33 GMT
EXPOSE 9080 9443
# Thu, 01 Jun 2023 01:29:33 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 01 Jun 2023 01:29:34 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904a0c815c072ccdf47e2b629d60ff91ad3ae9a1485d39c406b7c5e846233b1c`  
		Last Modified: Tue, 18 Apr 2023 01:29:20 GMT  
		Size: 15.7 MB (15693377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0035bd1ad5e27c9f579a780ebe65a17fa3b05ea00b73d6a266bb72271fa9ae4d`  
		Last Modified: Wed, 31 May 2023 23:55:19 GMT  
		Size: 50.2 MB (50170377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cade5ea768fba19782b48f6c450de05b34f9e2a638d75fdf13b5173e7634ba35`  
		Last Modified: Wed, 31 May 2023 23:55:14 GMT  
		Size: 4.3 MB (4333467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e88d2ef05de50c6cf496677d8b9c72c90882941d401254e606d4dc0e5b0bcc8`  
		Last Modified: Thu, 01 Jun 2023 01:43:16 GMT  
		Size: 8.2 KB (8223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38b8b7f341214fe99880afd5c29c75e745939837b6bcd5ad13784c651049973`  
		Last Modified: Thu, 01 Jun 2023 01:43:15 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a166139d16e943798392ec76cbbaa59f9664fffe2341c5eee1b50f58b4bba08`  
		Last Modified: Thu, 01 Jun 2023 01:43:16 GMT  
		Size: 12.2 MB (12219673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39df9db7dc7e033debdb2f1d0380ed4288b59012f5cf56f772646b94aca99e5b`  
		Last Modified: Thu, 01 Jun 2023 01:43:15 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f771fb02c2ffc5ab216bf2eb8a6b63bb48f78175ba52f48ffad1c712fac2d11`  
		Last Modified: Thu, 01 Jun 2023 01:43:15 GMT  
		Size: 9.3 KB (9337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c2881cbe71c4e7ea71276387f5cb3103db1345180a61dcecc81375f70f510f`  
		Last Modified: Thu, 01 Jun 2023 01:43:15 GMT  
		Size: 2.6 MB (2555041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
