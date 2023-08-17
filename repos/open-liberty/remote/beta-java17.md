## `open-liberty:beta-java17`

```console
$ docker pull open-liberty@sha256:dc434d000b9dab189c3ca956f4e901bddeb7aaa5579eaac1b7f3dc72178ed4a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta-java17` - linux; amd64

```console
$ docker pull open-liberty@sha256:f3e4f6868a9603c6fd7560cea5ff2fe5748e0107f46e4bf80647e84551d759d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **469.9 MB (469863988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d562df80c2f98cc8b0b6130c9c0d1b21d6f0ddde18ee52fdc7acfb8a25a1fb1`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:47:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 15:47:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:51:28 GMT
ENV JAVA_VERSION=jdk-17.0.7+7_openj9-0.38.0
# Wed, 16 Aug 2023 15:52:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='601dba428fe9d9b5a883aaccbdd37f88c1fb0da2e5b5de65b40cf0a4a0e5fccb';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dee6b87258ceba918543956dddf97291cbc2735ffa0288d25239a07c7766d567';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ffda41aa8390d14edbce1775d652f0e4e779df025ac1404c1970802697963aab';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='ee08d6830990562fcc45bec336748390d15357028d3ca0cf4a78bcea7bdfaefe';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Aug 2023 15:52:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 15:52:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 16 Aug 2023 15:53:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 17 Aug 2023 08:12:03 GMT
USER root
# Thu, 17 Aug 2023 09:04:55 GMT
ARG LIBERTY_VERSION=23.0.0.8-beta
# Thu, 17 Aug 2023 09:04:55 GMT
ARG LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4
# Thu, 17 Aug 2023 09:04:55 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip
# Thu, 17 Aug 2023 09:04:55 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Thu, 17 Aug 2023 09:04:55 GMT
ARG OPENJ9_SCC=true
# Thu, 17 Aug 2023 09:04:55 GMT
ARG VERBOSE=false
# Thu, 17 Aug 2023 09:04:56 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=23.0.0.8-beta
# Thu, 17 Aug 2023 09:04:56 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Thu, 17 Aug 2023 09:04:56 GMT
COPY dir:0c9b294d41044aadfdfa715e426d188c2e110fe670ffece13814d3dccfec754e in /opt/ol/helpers 
# Thu, 17 Aug 2023 09:04:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 17 Aug 2023 09:04:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Thu, 17 Aug 2023 09:05:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 17 Aug 2023 09:05:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 17 Aug 2023 09:05:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Thu, 17 Aug 2023 09:05:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 17 Aug 2023 09:05:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 17 Aug 2023 09:05:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 17 Aug 2023 09:05:39 GMT
USER 1001
# Thu, 17 Aug 2023 09:05:39 GMT
EXPOSE 9080 9443
# Thu, 17 Aug 2023 09:05:39 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 17 Aug 2023 09:05:39 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3fd228352238bb1856524b5a72c3fc8010fcaf4d2e94b2b3f4fa5561a6566`  
		Last Modified: Wed, 16 Aug 2023 15:56:02 GMT  
		Size: 12.2 MB (12155838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e984c52399ca357e48b8b95d7ce8b16adea6a2cf2ba86cf59a671f57690f65`  
		Last Modified: Wed, 16 Aug 2023 15:57:49 GMT  
		Size: 48.5 MB (48538523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589c288ca0f22bf3c4836d433c4d4acec4f9c33354ae990a3df7c9f8db6544e1`  
		Last Modified: Wed, 16 Aug 2023 15:57:43 GMT  
		Size: 4.7 MB (4746675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aef30ccc70451c9872dbdeacd15be2bbf65459bf030dfb32a851f4bb37c68c`  
		Last Modified: Thu, 17 Aug 2023 09:11:17 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f264a28337ac8239703e134294ca31ac390b9b6d3ff3305d2b36cc617ebd121`  
		Last Modified: Thu, 17 Aug 2023 09:11:17 GMT  
		Size: 9.2 KB (9226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05bd7d2d0e36fc3bdeff53f7e904906909e6e55bd47b3d8de76524e47eb3ce8`  
		Last Modified: Thu, 17 Aug 2023 09:11:16 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d0a3031f0ae5efcdfe22507e60d147c3b4293cfc834a9e0792cace350b823f`  
		Last Modified: Thu, 17 Aug 2023 09:11:14 GMT  
		Size: 31.7 KB (31749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd431ea00382b90054904f1c379bef9bedcfd76e373215d495871dfe36de17b`  
		Last Modified: Thu, 17 Aug 2023 09:11:44 GMT  
		Size: 361.1 MB (361102600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e85ef2e739cf8e093f83c01e72b8d3bef682f781e21fc234f7ed8291607650`  
		Last Modified: Thu, 17 Aug 2023 09:11:14 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd7dc67d27efb3052c18e619eba50f088255e345151578287f3f13a86f3eeb4`  
		Last Modified: Thu, 17 Aug 2023 09:11:15 GMT  
		Size: 10.7 KB (10691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ecaaddcb1009180c73ffc8c8927dd33e05d66756661b52ec7c42fc98e0aa69`  
		Last Modified: Thu, 17 Aug 2023 09:11:17 GMT  
		Size: 12.8 MB (12828199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java17` - linux; arm64 variant v8

```console
$ docker pull open-liberty@sha256:a7b108a547801b6c18bf54ef023c2dc86c57212b3687463543081e7ae99bf6e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **464.9 MB (464876979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670122ce53ceff42932ceeb13f29b2a63b72465d44f8ff714ba72d63ea12ce38`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 14:30:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 14:30:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 14:33:56 GMT
ENV JAVA_VERSION=jdk-17.0.7+7_openj9-0.38.0
# Wed, 16 Aug 2023 14:35:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='601dba428fe9d9b5a883aaccbdd37f88c1fb0da2e5b5de65b40cf0a4a0e5fccb';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dee6b87258ceba918543956dddf97291cbc2735ffa0288d25239a07c7766d567';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ffda41aa8390d14edbce1775d652f0e4e779df025ac1404c1970802697963aab';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='ee08d6830990562fcc45bec336748390d15357028d3ca0cf4a78bcea7bdfaefe';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Aug 2023 14:35:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 14:35:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 16 Aug 2023 14:35:42 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 16 Aug 2023 16:15:30 GMT
USER root
# Wed, 16 Aug 2023 16:39:15 GMT
ARG LIBERTY_VERSION=23.0.0.8-beta
# Wed, 16 Aug 2023 16:39:15 GMT
ARG LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4
# Wed, 16 Aug 2023 16:39:15 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip
# Wed, 16 Aug 2023 16:39:16 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Wed, 16 Aug 2023 16:39:16 GMT
ARG OPENJ9_SCC=true
# Wed, 16 Aug 2023 16:39:16 GMT
ARG VERBOSE=false
# Wed, 16 Aug 2023 16:39:16 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=23.0.0.8-beta
# Wed, 16 Aug 2023 16:39:16 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Wed, 16 Aug 2023 16:39:16 GMT
COPY dir:0c9b294d41044aadfdfa715e426d188c2e110fe670ffece13814d3dccfec754e in /opt/ol/helpers 
# Wed, 16 Aug 2023 16:39:16 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 16 Aug 2023 16:39:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Wed, 16 Aug 2023 16:39:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 16 Aug 2023 16:39:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 16 Aug 2023 16:39:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Wed, 16 Aug 2023 16:39:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 16 Aug 2023 16:39:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 16 Aug 2023 16:39:55 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 16 Aug 2023 16:39:55 GMT
USER 1001
# Wed, 16 Aug 2023 16:39:55 GMT
EXPOSE 9080 9443
# Wed, 16 Aug 2023 16:39:55 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 16 Aug 2023 16:39:55 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac60ed8a72576022d43698a13e953c7c74dac694b1a5a12ed5cebf1ae17c140`  
		Last Modified: Wed, 16 Aug 2023 14:38:10 GMT  
		Size: 12.1 MB (12113460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7016a60878d25d7d670b73380f64c3c45a8a97992c977361023b6aff47e9320`  
		Last Modified: Wed, 16 Aug 2023 14:39:49 GMT  
		Size: 46.5 MB (46514261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5d705eddd7c4128ce13ef6e4b3985796c1ab1e400293d0d0ca408bf0c0ef1c`  
		Last Modified: Wed, 16 Aug 2023 14:39:44 GMT  
		Size: 4.6 MB (4608546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381db76cabf1c3cab5debc19dd28c2511ae6becb8b864466ead78e1665a3b3e`  
		Last Modified: Wed, 16 Aug 2023 16:45:02 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d4aaaeccc30bae52d75581be9c47c313a3bdcbf8826e2ebf9c69c21308ed52`  
		Last Modified: Wed, 16 Aug 2023 16:45:02 GMT  
		Size: 9.2 KB (9222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7566ab56d5957977801e42516a523946b69616e2b99401ad19f69f3ce77c18c`  
		Last Modified: Wed, 16 Aug 2023 16:45:02 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3b91782435b7a1206534d0419bc2f495ae6c36abf39733c3480e6321faaed1`  
		Last Modified: Wed, 16 Aug 2023 16:45:00 GMT  
		Size: 42.3 KB (42322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4476b63d710604f02220f6d8d518f7c70473830c4651f595cf1ffa756e0dd30e`  
		Last Modified: Wed, 16 Aug 2023 16:45:20 GMT  
		Size: 361.1 MB (361104180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6636a066362b514879895901131eaff8aaaec9394a00f285168d812b8d1c816`  
		Last Modified: Wed, 16 Aug 2023 16:45:00 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d004195ee2a6fa99f15857be04d4723156f8abfdea2da31f5d8810d059caba2`  
		Last Modified: Wed, 16 Aug 2023 16:45:00 GMT  
		Size: 10.7 KB (10689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedf5c238c2c0de6ec98e44da9c8fed53c3397d48927e9ebd1867735a2141f9f`  
		Last Modified: Wed, 16 Aug 2023 16:45:02 GMT  
		Size: 12.1 MB (12079866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java17` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b7c87aea14677312716581126d1129faaea5910e6eac308f93e0f7820f6bae01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **474.3 MB (474305343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a3652172d82af454855436fd66ff929fbe1d2243196d60ae22d55789afe62a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 07:53:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 17 Aug 2023 07:53:44 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:58:10 GMT
ENV JAVA_VERSION=jdk-17.0.7+7_openj9-0.38.0
# Thu, 17 Aug 2023 07:59:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='601dba428fe9d9b5a883aaccbdd37f88c1fb0da2e5b5de65b40cf0a4a0e5fccb';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dee6b87258ceba918543956dddf97291cbc2735ffa0288d25239a07c7766d567';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ffda41aa8390d14edbce1775d652f0e4e779df025ac1404c1970802697963aab';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='ee08d6830990562fcc45bec336748390d15357028d3ca0cf4a78bcea7bdfaefe';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 17 Aug 2023 07:59:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 07:59:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 17 Aug 2023 08:00:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 17 Aug 2023 11:27:51 GMT
USER root
# Thu, 17 Aug 2023 13:18:53 GMT
ARG LIBERTY_VERSION=23.0.0.8-beta
# Thu, 17 Aug 2023 13:18:54 GMT
ARG LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4
# Thu, 17 Aug 2023 13:18:54 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip
# Thu, 17 Aug 2023 13:18:54 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Thu, 17 Aug 2023 13:18:55 GMT
ARG OPENJ9_SCC=true
# Thu, 17 Aug 2023 13:18:55 GMT
ARG VERBOSE=false
# Thu, 17 Aug 2023 13:18:55 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=23.0.0.8-beta
# Thu, 17 Aug 2023 13:18:55 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Thu, 17 Aug 2023 13:18:56 GMT
COPY dir:0c9b294d41044aadfdfa715e426d188c2e110fe670ffece13814d3dccfec754e in /opt/ol/helpers 
# Thu, 17 Aug 2023 13:18:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 17 Aug 2023 13:18:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Thu, 17 Aug 2023 13:19:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 17 Aug 2023 13:19:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 17 Aug 2023 13:19:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Thu, 17 Aug 2023 13:19:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 17 Aug 2023 13:20:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 17 Aug 2023 13:20:22 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 17 Aug 2023 13:20:23 GMT
USER 1001
# Thu, 17 Aug 2023 13:20:23 GMT
EXPOSE 9080 9443
# Thu, 17 Aug 2023 13:20:24 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 17 Aug 2023 13:20:24 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b5ceb7dfda582574a06a918e899d7d9019dd9005b084e06b6d57c5a53131`  
		Last Modified: Thu, 17 Aug 2023 08:04:07 GMT  
		Size: 12.9 MB (12895032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ec8bd5af4adac245260a1a4a0e274e2f1d37859a13e224cc89dcae57d43e98`  
		Last Modified: Thu, 17 Aug 2023 08:07:03 GMT  
		Size: 49.6 MB (49646565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32926c029db13c035efe7baa107af2378fcc1defe77d5f86e2a87409aa42b5bc`  
		Last Modified: Thu, 17 Aug 2023 08:06:52 GMT  
		Size: 3.8 MB (3751119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be04779319610417832aca35d059a4c33c740c73a1bee2ed02fd1d4c8b1480`  
		Last Modified: Thu, 17 Aug 2023 13:30:10 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590f5f6c0f2a75cc1d89bbaff86f1fdd0e7d2a48ea23044a48fe71e86830b08c`  
		Last Modified: Thu, 17 Aug 2023 13:30:10 GMT  
		Size: 9.2 KB (9226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6276edba9e2bc1ba3d87b37397a4e29ff8fd141d90a1870f5e578b678c4a905`  
		Last Modified: Thu, 17 Aug 2023 13:30:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd79233ef75588fe111412218c92c38b10daceb5a357f63cd4254a3b7c2c2f0b`  
		Last Modified: Thu, 17 Aug 2023 13:30:08 GMT  
		Size: 36.5 KB (36496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b586ea61771a21b4af03c23b8102fe9bbadb99308aab9903f06e63a9f26b77b5`  
		Last Modified: Thu, 17 Aug 2023 13:30:36 GMT  
		Size: 361.1 MB (361103162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83feee7861de3a0fdaf934fd150bf2412835401b12345c57ad748f6cf592708c`  
		Last Modified: Thu, 17 Aug 2023 13:30:08 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40cb464b2b603f6f9f4177ffa5c1af95a6a548f7606ef950c2363562a77ab9c`  
		Last Modified: Thu, 17 Aug 2023 13:30:07 GMT  
		Size: 10.7 KB (10708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352b5690c4cdc4db122c666f68f884f35b919fe58e92bb818915ef21b3a880c2`  
		Last Modified: Thu, 17 Aug 2023 13:30:10 GMT  
		Size: 11.1 MB (11137783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java17` - linux; s390x

```console
$ docker pull open-liberty@sha256:29efadc44322acb5dcfa9234992ad5e79f566c2c4118f2b54bf687bfa40f7894
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.1 MB (467126562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13860487687637f3cf259df308a4bd1ac6b1f33252a8ca01987622173c8f93c4`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 09:23:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 09:23:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:27:48 GMT
ENV JAVA_VERSION=jdk-17.0.7+7_openj9-0.38.0
# Wed, 16 Aug 2023 09:29:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='601dba428fe9d9b5a883aaccbdd37f88c1fb0da2e5b5de65b40cf0a4a0e5fccb';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_aarch64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dee6b87258ceba918543956dddf97291cbc2735ffa0288d25239a07c7766d567';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_ppc64le_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ffda41aa8390d14edbce1775d652f0e4e779df025ac1404c1970802697963aab';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_x64_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        s390x)          ESUM='ee08d6830990562fcc45bec336748390d15357028d3ca0cf4a78bcea7bdfaefe';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.7%2B7_openj9-0.38.0/ibm-semeru-open-jre_s390x_linux_17.0.7_7_openj9-0.38.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Aug 2023 09:29:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:29:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 16 Aug 2023 09:29:43 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 16 Aug 2023 17:46:09 GMT
USER root
# Wed, 16 Aug 2023 17:46:09 GMT
ARG LIBERTY_VERSION=23.0.0.8-beta
# Wed, 16 Aug 2023 17:46:09 GMT
ARG LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4
# Wed, 16 Aug 2023 17:46:09 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip
# Wed, 16 Aug 2023 17:46:10 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Wed, 16 Aug 2023 17:46:10 GMT
ARG OPENJ9_SCC=true
# Wed, 16 Aug 2023 17:46:10 GMT
ARG VERBOSE=false
# Wed, 16 Aug 2023 17:46:10 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=23.0.0.8-beta
# Wed, 16 Aug 2023 17:46:10 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Wed, 16 Aug 2023 17:46:10 GMT
COPY dir:0c9b294d41044aadfdfa715e426d188c2e110fe670ffece13814d3dccfec754e in /opt/ol/helpers 
# Wed, 16 Aug 2023 17:46:10 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 16 Aug 2023 17:46:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Wed, 16 Aug 2023 17:46:31 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 16 Aug 2023 17:46:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 16 Aug 2023 17:46:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Wed, 16 Aug 2023 17:46:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 16 Aug 2023 17:46:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/23.0.0.8-beta/openliberty-runtime-23.0.0.8-beta.zip LIBERTY_SHA=7bd9ae608dec65669dde34c56d93cee4b964cda4 LIBERTY_VERSION=23.0.0.8-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 16 Aug 2023 17:47:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 16 Aug 2023 17:47:00 GMT
USER 1001
# Wed, 16 Aug 2023 17:47:00 GMT
EXPOSE 9080 9443
# Wed, 16 Aug 2023 17:47:00 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 16 Aug 2023 17:47:00 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33878ed31a5f2ae2ce7e393a139a1e3266bdd76a60af22203b6d4fcd73343dd7`  
		Last Modified: Wed, 16 Aug 2023 09:33:07 GMT  
		Size: 12.2 MB (12199840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7c2636dc28310a3cedbcb73121064687568aef15bdba057a998869dbc4f6d`  
		Last Modified: Wed, 16 Aug 2023 09:34:45 GMT  
		Size: 47.6 MB (47567688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e629a3d024cac4080091fec593dacfc526207622578c53fca2c9e7b7c7e61b0a`  
		Last Modified: Wed, 16 Aug 2023 09:34:39 GMT  
		Size: 5.0 MB (4953592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7057bc3b7680c0d052b7547bf9cab5a2eba7bd713f8cee961913df47dc739a`  
		Last Modified: Wed, 16 Aug 2023 17:54:51 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d09745bbb95ee5e29cdd959289b4257cab450ccb0cd8fe569abf263bd4ed5e`  
		Last Modified: Wed, 16 Aug 2023 17:54:51 GMT  
		Size: 9.2 KB (9221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e56892f767c80442cf5e81c3fed61f662eb0ff08277c28f7ff5bc1e954d605`  
		Last Modified: Wed, 16 Aug 2023 17:54:51 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9b00e4f5fa37e98a381685c15362208420b8949bd5fef12b0cf34ae1b46cb`  
		Last Modified: Wed, 16 Aug 2023 17:54:49 GMT  
		Size: 33.1 KB (33113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e6c1968988cc0f54a2aa90db40bae9d08dd5d9e09dbd593913b4bba75629a2`  
		Last Modified: Wed, 16 Aug 2023 17:55:05 GMT  
		Size: 361.1 MB (361102820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ddf734ecef3abcca112a7be513bc699135c3c82ea1124ba590da44dd07f95f`  
		Last Modified: Wed, 16 Aug 2023 17:54:50 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ecebf71d7d41c48e1a46573eb41c4517db64c7a0674d849f595793ab2471d5`  
		Last Modified: Wed, 16 Aug 2023 17:54:50 GMT  
		Size: 10.7 KB (10688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3550d38322b712e8740c7db79366d4a5b9175c71642de862579fe937b73a22`  
		Last Modified: Wed, 16 Aug 2023 17:54:51 GMT  
		Size: 12.6 MB (12602698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
