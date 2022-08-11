## `open-liberty:beta-java11`

```console
$ docker pull open-liberty@sha256:01b983ac5f24a21f26e04626c3cb953479293cf2ac3df1ab3ed415c0d12e6564
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta-java11` - linux; amd64

```console
$ docker pull open-liberty@sha256:e93913e41ad04349eb92a16ee7652fcbc570da9077d5eeb780982194a6fb8ceb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.6 MB (426598320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8732f741c7527008ea80f910eba6d3e01ae711db0bf20e234e9c733e7f855728`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 22:45:19 GMT
ENV JAVA_VERSION=jdk-11.0.16+8_openj9-0.33.0
# Wed, 10 Aug 2022 22:47:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='49dc05a3e9f3f99c5f8fa466261aa3e33a753694c67cabfa7d3f682e5a2e3685';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='552da889577571881ac58eb06877ca2fdadc12397f433b553b319674ee10a02d';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ba09711193b8b8664478f3f949b5320232f65c1bdf61f32a885d84de73c02767';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='edfccd071e4276c51884cd89522b3be21fd2e44612f98f7a7d3dceb0c339a391';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 22:47:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:47:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 22:47:46 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 23:23:49 GMT
ARG LIBERTY_VERSION=22.0.0.9-beta
# Wed, 10 Aug 2022 23:23:49 GMT
ARG LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48
# Wed, 10 Aug 2022 23:23:49 GMT
ARG LIBERTY_BUILD_LABEL=cl220820220719-1056
# Wed, 10 Aug 2022 23:23:50 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip
# Wed, 10 Aug 2022 23:23:50 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 10 Aug 2022 23:23:50 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 10 Aug 2022 23:23:50 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:23:50 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 23:23:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.9-beta
# Wed, 10 Aug 2022 23:23:50 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 10 Aug 2022 23:23:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 10 Aug 2022 23:24:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 10 Aug 2022 23:24:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:24:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 23:24:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 10 Aug 2022 23:24:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 10 Aug 2022 23:24:34 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 23:24:34 GMT
USER 1001
# Wed, 10 Aug 2022 23:24:34 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 23:24:34 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 23:24:34 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398d776e32fac0ec8c2698a6d7bc5d81c5d35de32a68fb2d7882e0f46b73fd37`  
		Last Modified: Tue, 02 Aug 2022 19:13:20 GMT  
		Size: 16.0 MB (16029939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae1b8d04e3b180095582892e267b24b70e7d91e19764b8dc0f9d4445b894cbf`  
		Last Modified: Wed, 10 Aug 2022 22:59:11 GMT  
		Size: 48.0 MB (48030809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd248a0b366f0ee9b5c5a6a6d9a8d0a9d4f20213a539fc3a11117b3f103405e5`  
		Last Modified: Wed, 10 Aug 2022 22:59:05 GMT  
		Size: 4.2 MB (4225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede2fc7506efceb398bce8bd50bdc49d552da3d0236bdf64d7cf56b67be318c0`  
		Last Modified: Wed, 10 Aug 2022 23:36:40 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cc9a8eaed1b4221ae0ace19b8b8036e17cbb3121feb75d0352095f55affa51`  
		Last Modified: Wed, 10 Aug 2022 23:36:37 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd74622944911352b81b5f2d33c70ad22eb1f0ace4ddc48800b5b530068ed87`  
		Last Modified: Wed, 10 Aug 2022 23:36:53 GMT  
		Size: 316.0 MB (315973167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef015a0a610dbc1fc77b7b5c9046a6ddf8a7b1f024681b76e2ab70fa484a054`  
		Last Modified: Wed, 10 Aug 2022 23:36:38 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f17461db0729530adf2cdb6edbff05b3ef28d762996e3995b754d71da8e21f`  
		Last Modified: Wed, 10 Aug 2022 23:36:37 GMT  
		Size: 10.0 KB (10043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70687aec0da33c9c75924d33f30dd7c083376d59a805b16daccb528c0f75f48d`  
		Last Modified: Wed, 10 Aug 2022 23:36:40 GMT  
		Size: 13.7 MB (13746490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:d86365a6915cc239c7e2e0775949e0647a1e6078b6207138cd2f7a1567df9eec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.9 MB (430944515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22cca8d94ac892998c7bb3ec74c141f62565f1bd45e570a5d7060423a965bebf`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:18:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 03 Aug 2022 03:20:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 22:21:02 GMT
ENV JAVA_VERSION=jdk-11.0.16+8_openj9-0.33.0
# Wed, 10 Aug 2022 22:23:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='49dc05a3e9f3f99c5f8fa466261aa3e33a753694c67cabfa7d3f682e5a2e3685';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='552da889577571881ac58eb06877ca2fdadc12397f433b553b319674ee10a02d';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ba09711193b8b8664478f3f949b5320232f65c1bdf61f32a885d84de73c02767';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='edfccd071e4276c51884cd89522b3be21fd2e44612f98f7a7d3dceb0c339a391';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 22:23:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:23:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 22:24:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 23:02:24 GMT
ARG LIBERTY_VERSION=22.0.0.9-beta
# Wed, 10 Aug 2022 23:02:24 GMT
ARG LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48
# Wed, 10 Aug 2022 23:02:24 GMT
ARG LIBERTY_BUILD_LABEL=cl220820220719-1056
# Wed, 10 Aug 2022 23:02:24 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip
# Wed, 10 Aug 2022 23:02:25 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 10 Aug 2022 23:02:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 10 Aug 2022 23:02:25 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:02:26 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 23:02:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.9-beta
# Wed, 10 Aug 2022 23:02:26 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 10 Aug 2022 23:02:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 10 Aug 2022 23:03:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 10 Aug 2022 23:03:07 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:03:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 23:03:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 10 Aug 2022 23:03:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 10 Aug 2022 23:03:53 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 23:03:54 GMT
USER 1001
# Wed, 10 Aug 2022 23:03:54 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 23:03:54 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 23:03:55 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93d2375ba0032ebd673deba460fc14719ca1d2863b8d267e076565f71f6a0a6`  
		Last Modified: Wed, 03 Aug 2022 03:33:39 GMT  
		Size: 17.2 MB (17202740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42098800e9ee745505891252fbc0d15abbf06d7f6374f62e952ce24d02c1914b`  
		Last Modified: Wed, 10 Aug 2022 22:39:49 GMT  
		Size: 48.8 MB (48769826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbea86f2676c04f50d4d38175ea4a61be932c3f1da53385ac6992d423194816b`  
		Last Modified: Wed, 10 Aug 2022 22:39:38 GMT  
		Size: 3.4 MB (3425318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf6e931071e3c5c81f9d33f1e46f61ddd5b3fb2dadd7beb3964b9da8d0f7a9a`  
		Last Modified: Wed, 10 Aug 2022 23:28:23 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a568c1fb6c2e8c2dbcce3b6adcfd4f0f9f68e7c943b85c8e2aea08ce7606294`  
		Last Modified: Wed, 10 Aug 2022 23:28:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555f4c9ff95e763106b3219f864106ce9d392704b70807f2fc60be7e137b4c35`  
		Last Modified: Wed, 10 Aug 2022 23:28:47 GMT  
		Size: 316.0 MB (315973696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94275609eab43c2459d4db7fd67dbebf83b482f3fee29aaa0e779374ef4df68`  
		Last Modified: Wed, 10 Aug 2022 23:28:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dee218b9852aa357d65e420782f6538897f471e88d87ac6a5d44d5d5d45358`  
		Last Modified: Wed, 10 Aug 2022 23:28:21 GMT  
		Size: 10.1 KB (10062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbaeb246167c8dbfaafa2b0264ce4d10bd9d5ffa6a4455cfbad7bb88dca1edb`  
		Last Modified: Wed, 10 Aug 2022 23:28:24 GMT  
		Size: 12.3 MB (12257457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; s390x

```console
$ docker pull open-liberty@sha256:bc89717aa126d1eb0f0576036270f9a5abf331c29a9790706069bf27fa58086b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.6 MB (424562910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c119bf5538864d05e388566a4d3e122d344b47ac5b40bda62a51df8ab9cddc6b`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 21:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.16+8_openj9-0.33.0
# Wed, 10 Aug 2022 21:45:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='49dc05a3e9f3f99c5f8fa466261aa3e33a753694c67cabfa7d3f682e5a2e3685';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='552da889577571881ac58eb06877ca2fdadc12397f433b553b319674ee10a02d';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ba09711193b8b8664478f3f949b5320232f65c1bdf61f32a885d84de73c02767';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='edfccd071e4276c51884cd89522b3be21fd2e44612f98f7a7d3dceb0c339a391';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 21:45:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 21:45:21 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 21:46:02 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 22:33:26 GMT
ARG LIBERTY_VERSION=22.0.0.9-beta
# Wed, 10 Aug 2022 22:33:26 GMT
ARG LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48
# Wed, 10 Aug 2022 22:33:26 GMT
ARG LIBERTY_BUILD_LABEL=cl220820220719-1056
# Wed, 10 Aug 2022 22:33:26 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip
# Wed, 10 Aug 2022 22:33:26 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 10 Aug 2022 22:33:27 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 10 Aug 2022 22:33:27 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 22:33:27 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 22:33:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.9-beta
# Wed, 10 Aug 2022 22:33:27 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 10 Aug 2022 22:33:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 10 Aug 2022 22:33:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 10 Aug 2022 22:33:48 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 10 Aug 2022 22:33:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 22:33:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 10 Aug 2022 22:34:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.9-beta/openliberty-runtime-22.0.0.9-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=f3520ad919d8d3a21d16f9dc74327ca151952f48 LIBERTY_VERSION=22.0.0.9-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 10 Aug 2022 22:34:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 22:34:13 GMT
USER 1001
# Wed, 10 Aug 2022 22:34:14 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 22:34:14 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 22:34:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204f6f9c0aa5d9c3e1300660817d3dd41177073448243d9ccc18a39c3f14083a`  
		Last Modified: Tue, 02 Aug 2022 12:52:19 GMT  
		Size: 15.7 MB (15730128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8789b0a8047984a2b7ccee4b3a6081deb0fe29bda6be096c6f02bea19fc78ba6`  
		Last Modified: Wed, 10 Aug 2022 21:57:01 GMT  
		Size: 47.6 MB (47591346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e87136408d5c44592bc0724a77c4a077d72029332252bbfc32bfee89ea4d`  
		Last Modified: Wed, 10 Aug 2022 21:56:55 GMT  
		Size: 4.3 MB (4347894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5343c0bb52e55799fd6adea3636cbaf1382a44435fdcc4b169677fa7a305d329`  
		Last Modified: Wed, 10 Aug 2022 22:49:08 GMT  
		Size: 8.6 KB (8553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856fbc0970dcba9e282c43dc1be5078353a9884ce77d4d015f66027f102f6015`  
		Last Modified: Wed, 10 Aug 2022 22:49:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3a4f6a085889a1a3d55423e14ccbc65abdca1159868cc4b0bc6b9980189004`  
		Last Modified: Wed, 10 Aug 2022 22:49:20 GMT  
		Size: 316.0 MB (315973299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc6c4e5cdd54518ae4f095636210000a8251449bbd723a43fa19a7834d37e03`  
		Last Modified: Wed, 10 Aug 2022 22:49:07 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80ba847e2c8d982e38b6eb2cac10d470dc0a673d0ead43152a860af7e3d766a`  
		Last Modified: Wed, 10 Aug 2022 22:49:07 GMT  
		Size: 10.0 KB (10042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59c44d7baa7c167c416dfdaff419c47f13846619883bc66f7f0063198e1ae`  
		Last Modified: Wed, 10 Aug 2022 22:49:09 GMT  
		Size: 13.9 MB (13854772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
