## `open-liberty:kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:11a6c35b2bc94caa34e6ac840fe2d15062a075ab41031c4677ed5a798a66e1be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:bf0b9d1cc27c4e9e10f7263786c4c4c9733c1e4b6b885801150deb00dc0c3f1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113145293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bfdd10f52592fb670110ad841a078be6f25b064d53a2c958689f5ea59a7db2`
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
# Wed, 10 Aug 2022 22:41:57 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.0
# Wed, 10 Aug 2022 22:43:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='03caff41622e84a6e7fa66a225414a9b6eefb38dd215f830cae0bc4bbfc55b5c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7cd45d320f9ad4e00e78f96478a1a9d47847df4a0a6bce0aaff9ad7e7d997703';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='0d4fe62716b9da2ccce324b5b46d57e8d47e5dfb5d128f87e16135ee9bc36cdc';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.0.tar.gz';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='38f97a42440f50e9dc59638401d6ae3f730aff32ee95c82b26def68d9602f66b';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 22:43:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:43:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 22:44:23 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 23:25:26 GMT
ARG LIBERTY_VERSION=22.0.0.8
# Wed, 10 Aug 2022 23:25:26 GMT
ARG LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730
# Wed, 10 Aug 2022 23:25:26 GMT
ARG LIBERTY_BUILD_LABEL=cl220820220719-1056
# Wed, 10 Aug 2022 23:25:26 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip
# Wed, 10 Aug 2022 23:25:26 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 10 Aug 2022 23:25:26 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 10 Aug 2022 23:25:26 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:25:26 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 23:25:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.8
# Wed, 10 Aug 2022 23:25:27 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 10 Aug 2022 23:25:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 10 Aug 2022 23:25:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 10 Aug 2022 23:25:32 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:25:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 23:25:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 10 Aug 2022 23:25:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 10 Aug 2022 23:25:40 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 23:25:40 GMT
USER 1001
# Wed, 10 Aug 2022 23:25:40 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 23:25:40 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 23:25:40 GMT
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
	-	`sha256:80c2eb6b2043eb9f1b45044036c4c9d5ffeafaf1b5cfcbe1a6264939d237dc10`  
		Last Modified: Wed, 10 Aug 2022 22:57:50 GMT  
		Size: 50.1 MB (50065031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bc1f3394e59190ffa1b2bf45922b5bfdfdef95f576da7f242ed4caccb59701`  
		Last Modified: Wed, 10 Aug 2022 22:57:45 GMT  
		Size: 4.2 MB (4206026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fe80dfd618b5d61d95b2b01905d8b9255f2717f39b4ca18d35cd4475145d7`  
		Last Modified: Wed, 10 Aug 2022 23:37:25 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd573f3b45c3d4376836b3cd0292a853336f2cf6dd36d6cd2a1a6e3ffec6e82`  
		Last Modified: Wed, 10 Aug 2022 23:37:22 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd523c2a68e7f9343e6be87e6f21efaa09dae3a18cadcdd60a60c4b57d0f31f2`  
		Last Modified: Wed, 10 Aug 2022 23:37:23 GMT  
		Size: 11.7 MB (11733006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ee2ba81846635f00c2c6dfbf5d683ac5707382646153f7b9754fd2dc7575ed`  
		Last Modified: Wed, 10 Aug 2022 23:37:22 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d397882986b264c4173a849f0a64166751702d3a35ad576dad90c755062c8a`  
		Last Modified: Wed, 10 Aug 2022 23:37:22 GMT  
		Size: 9.2 KB (9207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3d05b80c3cd7f0545fb2fc3d9aa5400e5d37857f1f17b962d2370271a2ab4`  
		Last Modified: Wed, 10 Aug 2022 23:37:23 GMT  
		Size: 2.5 MB (2520189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:04808ea6169d4b523f007fc4dd5cb0a763213369d524fdd263f06bb660aae068
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118845017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81796db116303337465c6f9883c7145564a8eddd61472aece73b5561df337980`
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
# Wed, 10 Aug 2022 22:16:57 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.0
# Wed, 10 Aug 2022 22:19:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='03caff41622e84a6e7fa66a225414a9b6eefb38dd215f830cae0bc4bbfc55b5c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7cd45d320f9ad4e00e78f96478a1a9d47847df4a0a6bce0aaff9ad7e7d997703';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='0d4fe62716b9da2ccce324b5b46d57e8d47e5dfb5d128f87e16135ee9bc36cdc';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.0.tar.gz';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='38f97a42440f50e9dc59638401d6ae3f730aff32ee95c82b26def68d9602f66b';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 22:19:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:19:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 22:19:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 23:05:44 GMT
ARG LIBERTY_VERSION=22.0.0.8
# Wed, 10 Aug 2022 23:05:44 GMT
ARG LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730
# Wed, 10 Aug 2022 23:05:44 GMT
ARG LIBERTY_BUILD_LABEL=cl220820220719-1056
# Wed, 10 Aug 2022 23:05:44 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip
# Wed, 10 Aug 2022 23:05:45 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 10 Aug 2022 23:05:45 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 10 Aug 2022 23:05:45 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:05:46 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 23:05:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.8
# Wed, 10 Aug 2022 23:05:46 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 10 Aug 2022 23:05:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 10 Aug 2022 23:05:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 10 Aug 2022 23:05:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 10 Aug 2022 23:05:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 23:05:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 10 Aug 2022 23:06:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 10 Aug 2022 23:06:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 23:06:09 GMT
USER 1001
# Wed, 10 Aug 2022 23:06:09 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 23:06:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 23:06:10 GMT
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
	-	`sha256:1c5f5048787fa34a5c4dfcd563c6a41f9e97ec32f46878abd7345467bdecb05f`  
		Last Modified: Wed, 10 Aug 2022 22:37:49 GMT  
		Size: 50.5 MB (50543168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f127fb4369aa926d573d51546902c5a90a418e2fd1b65ac1c7ce923ec177ea2`  
		Last Modified: Wed, 10 Aug 2022 22:37:40 GMT  
		Size: 3.6 MB (3554083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36320c16d88671eda0784eb41161405582d898adf7b11e0f406ef86543aadafb`  
		Last Modified: Wed, 10 Aug 2022 23:29:34 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbcd3e5e7c5211d2ae2b33495c37d8832a082d86a3679891b8cffb0148aed64`  
		Last Modified: Wed, 10 Aug 2022 23:29:32 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fe6287b2adf7e20c61a95701dc76739f708b41d4ff60006259553169b9e4d7`  
		Last Modified: Wed, 10 Aug 2022 23:29:33 GMT  
		Size: 11.7 MB (11733541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e5582b7f9e26de48d2db7f926dba5d991c89520f8f897ccc09701e02975a54`  
		Last Modified: Wed, 10 Aug 2022 23:29:32 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf75748ad6e5edc4eee7a6ea1fd60ae096240458d5097be61076cb5f5872847`  
		Last Modified: Wed, 10 Aug 2022 23:29:32 GMT  
		Size: 9.2 KB (9211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac42d58094a9a4a005e73abca964c1c2bd0e78df9093fe1b7c55c6a5270f3a7`  
		Last Modified: Wed, 10 Aug 2022 23:29:33 GMT  
		Size: 2.5 MB (2497616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:a216479e567d1cdb6e48a9a062985c3e9176d3de4ec4fd70f4d7b8509a0fb068
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111422708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baab70140aba58968f7684c55395eebc50d9f3f979b1884715a63a2dfa5a8d6e`
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
# Wed, 10 Aug 2022 21:41:56 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.0
# Wed, 10 Aug 2022 21:43:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='03caff41622e84a6e7fa66a225414a9b6eefb38dd215f830cae0bc4bbfc55b5c';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7cd45d320f9ad4e00e78f96478a1a9d47847df4a0a6bce0aaff9ad7e7d997703';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='0d4fe62716b9da2ccce324b5b46d57e8d47e5dfb5d128f87e16135ee9bc36cdc';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.0.tar.gz';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='38f97a42440f50e9dc59638401d6ae3f730aff32ee95c82b26def68d9602f66b';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_8u345b01_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 21:43:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 21:43:17 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 21:43:55 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 22:35:22 GMT
ARG LIBERTY_VERSION=22.0.0.8
# Wed, 10 Aug 2022 22:35:23 GMT
ARG LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730
# Wed, 10 Aug 2022 22:35:23 GMT
ARG LIBERTY_BUILD_LABEL=cl220820220719-1056
# Wed, 10 Aug 2022 22:35:23 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip
# Wed, 10 Aug 2022 22:35:23 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 10 Aug 2022 22:35:23 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 10 Aug 2022 22:35:23 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 22:35:24 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 22:35:24 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.8
# Wed, 10 Aug 2022 22:35:24 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 10 Aug 2022 22:35:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 10 Aug 2022 22:35:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 10 Aug 2022 22:35:29 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 10 Aug 2022 22:35:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 22:35:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 10 Aug 2022 22:35:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220820220719-1056 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.8/openliberty-kernel-22.0.0.8.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5ed6c43b8d3047b55c25495094491817359eb730 LIBERTY_VERSION=22.0.0.8 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 10 Aug 2022 22:35:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 22:35:36 GMT
USER 1001
# Wed, 10 Aug 2022 22:35:36 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 22:35:36 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 22:35:37 GMT
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
	-	`sha256:eb43598fb035bfe35e992aa9b11dd5f88e0f6766b97711225918166fbfcd7939`  
		Last Modified: Wed, 10 Aug 2022 21:54:02 GMT  
		Size: 50.0 MB (49976331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6912287d4ff45ee5b6b0fb5b17700ed01d47313b2f7534be081469b0d3d74512`  
		Last Modified: Wed, 10 Aug 2022 21:53:53 GMT  
		Size: 4.3 MB (4338434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f181719766ea87e40cadc711b3cd3627faa6c80db23d122e725580511adeaa`  
		Last Modified: Wed, 10 Aug 2022 22:49:44 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72a7fb0332f989af6ddbf78b625b3261d5b7f9e85936309e5eca8ddf77d1769`  
		Last Modified: Wed, 10 Aug 2022 22:49:43 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5644caedc698c84c92aee77a18a760c05feacad9c2234e5c6ae4040fdcec414`  
		Last Modified: Wed, 10 Aug 2022 22:49:43 GMT  
		Size: 11.7 MB (11733104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e123d3dca66515dd7f71bfb0e334fbdbcfe42bf11e12e823de41e3d26f4427da`  
		Last Modified: Wed, 10 Aug 2022 22:49:43 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fb3e39b7d692ffe1e5cd60e79e4a89d76cf7e7aecda3b255a680a3bd99a8fd`  
		Last Modified: Wed, 10 Aug 2022 22:49:43 GMT  
		Size: 9.2 KB (9215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b619a6fe3ffbebd29098e82ab4b11eb522c3e3c128651319847c6207624dbd`  
		Last Modified: Wed, 10 Aug 2022 22:49:43 GMT  
		Size: 2.6 MB (2580829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
