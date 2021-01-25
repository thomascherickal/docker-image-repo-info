<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `open-liberty`

-	[`open-liberty:20.0.0.12-full-java11-openj9`](#open-liberty200012-full-java11-openj9)
-	[`open-liberty:20.0.0.12-full-java8-openj9`](#open-liberty200012-full-java8-openj9)
-	[`open-liberty:20.0.0.12-kernel-slim-java11-openj9`](#open-liberty200012-kernel-slim-java11-openj9)
-	[`open-liberty:20.0.0.12-kernel-slim-java8-openj9`](#open-liberty200012-kernel-slim-java8-openj9)
-	[`open-liberty:20.0.0.9-full-java8-openj9`](#open-liberty20009-full-java8-openj9)
-	[`open-liberty:20.0.0.9-kernel-java8-openj9`](#open-liberty20009-kernel-java8-openj9)
-	[`open-liberty:21.0.0.1-full-java11-openj9`](#open-liberty21001-full-java11-openj9)
-	[`open-liberty:21.0.0.1-full-java8-openj9`](#open-liberty21001-full-java8-openj9)
-	[`open-liberty:21.0.0.1-kernel-slim-java11-openj9`](#open-liberty21001-kernel-slim-java11-openj9)
-	[`open-liberty:21.0.0.1-kernel-slim-java8-openj9`](#open-liberty21001-kernel-slim-java8-openj9)
-	[`open-liberty:beta`](#open-libertybeta)
-	[`open-liberty:beta-java11`](#open-libertybeta-java11)
-	[`open-liberty:full`](#open-libertyfull)
-	[`open-liberty:full-java11-openj9`](#open-libertyfull-java11-openj9)
-	[`open-liberty:full-java8-openj9`](#open-libertyfull-java8-openj9)
-	[`open-liberty:kernel-slim`](#open-libertykernel-slim)
-	[`open-liberty:kernel-slim-java11-openj9`](#open-libertykernel-slim-java11-openj9)
-	[`open-liberty:kernel-slim-java8-openj9`](#open-libertykernel-slim-java8-openj9)
-	[`open-liberty:latest`](#open-libertylatest)

## `open-liberty:20.0.0.12-full-java11-openj9`

```console
$ docker pull open-liberty@sha256:c890cc586507f0f7979252cca708dc50554ff9fd656b152c4eda949998a2016c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.12-full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:8ac167d3164315d4fd74bef7d9122c3532f42544ed0957056825eb49aa5cf6ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.2 MB (279171024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca444551af85dd00b08e3cfc5fea00b3c589831ac2e4369aa4f839c1f7a282a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:25:27 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:27:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:27:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:27:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:28:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:28:53 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:53:49 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:53:49 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:53:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:53:49 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:53:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:54:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:54:01 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:54:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:54:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:54:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:54:42 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:54:43 GMT
USER 1001
# Tue, 24 Nov 2020 01:54:43 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:54:43 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:54:43 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c6ae47f01d1ca61746122b9b904e8cf3d3f16e048774c5c301b535c035c87`  
		Last Modified: Wed, 28 Oct 2020 17:40:51 GMT  
		Size: 42.8 MB (42770675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bffedeca141cd6b2ed75ae8a7aea20289574815afef5089ea410c4305532a8`  
		Last Modified: Wed, 28 Oct 2020 17:40:44 GMT  
		Size: 4.4 MB (4431006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26960407c3776c8b5df4a9fbf761863b267bef198b4fce4f1ef2bc52ab4a0980`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 8.5 KB (8516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e929c87ce24fca4109057fadaf4288c2fec5fa8189f17894b1aa512ea9095776`  
		Last Modified: Tue, 24 Nov 2020 01:57:56 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830cb5582179b38d8d635e7d9596337d35fe6bf586f1079eb6a48f7ce8a3b0bd`  
		Last Modified: Tue, 24 Nov 2020 01:58:07 GMT  
		Size: 173.6 MB (173562103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9acb0edaf613f391a8ea09d433c0257d011381b422f23886f5c9840c5865a1`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037abc0895b48f5936b240d870104a8720c29d0cd9eb9a27c614ab1643d026b6`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 9.9 KB (9900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9db8da445ba07b490b0394018ad9883786e4b1047f183caabc203fb2b0208b`  
		Last Modified: Tue, 24 Nov 2020 01:57:59 GMT  
		Size: 13.8 MB (13796295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:ad5f1845f680d430a69059362583d8cf15e5a40857c7705624d1d46e38dc7117
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.2 MB (283191950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:416dbec692ae7e5086385a69fbff91be75a5ed94c45dbe91e83029b74344c2ce`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:29:32 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:32:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:32:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:32:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:34:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:34:21 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:41:52 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:47:55 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 03:48:00 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:48:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 03:48:07 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:48:09 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:48:13 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:48:16 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:48:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:48:20 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:48:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:48:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:48:58 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:49:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:49:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:50:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:50:50 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:50:53 GMT
USER 1001
# Tue, 24 Nov 2020 03:50:57 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:51:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:51:10 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9518fb573dc23ad650fc0ea068af5f93f07e910761dbb8b83156f14d391027`  
		Last Modified: Wed, 28 Oct 2020 17:53:00 GMT  
		Size: 43.7 MB (43650458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7e2048088ed2d44960340a046c30cd88499c7356ea5d5da70160cb9286e6de`  
		Last Modified: Wed, 28 Oct 2020 17:52:52 GMT  
		Size: 3.5 MB (3464582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ca5f33c45bc1fb66d815593bed20c1fa116c2577117135a535b975e6d0669a`  
		Last Modified: Tue, 24 Nov 2020 03:59:45 GMT  
		Size: 8.5 KB (8549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c5b1d0f1062df749fafac658321c6e09b301a3bb5b4d2d353ba2e721fbb421`  
		Last Modified: Tue, 24 Nov 2020 03:59:41 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7066a36d28eb4dc8face0f1d38076e2d893d57d601a1ae4cc766f838b906d6a`  
		Last Modified: Tue, 24 Nov 2020 03:59:59 GMT  
		Size: 173.6 MB (173562818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fb888ec1de655aefa72caec26571dc95f30b98e5b733523bf02966728c8295`  
		Last Modified: Tue, 24 Nov 2020 03:59:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca8149a48aaf46787b9df7436786ec7c870640634a3947a72dd4e0c6b619af`  
		Last Modified: Tue, 24 Nov 2020 03:59:42 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b939e34871786a62e214174d2588eef1dbda71eb753de5aae93a05048e64d6`  
		Last Modified: Tue, 24 Nov 2020 03:59:46 GMT  
		Size: 12.0 MB (12009096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:cf8858f9efaa44ced868f90cd690c36f386073702faeff5ac20268392b385d55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.7 MB (275674712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82702e38a99d995b87e8195a1b9f3bce7c6281033b881d6bffbb7bc29cff87a0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:47:34 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:49:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:51:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:51:11 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:10 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:53:31 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:53:32 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:53:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:53:33 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:53:34 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:53:34 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:53:35 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:53:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:53:36 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:53:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:54:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:54:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:54:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:54:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:54:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:54:57 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:54:58 GMT
USER 1001
# Tue, 24 Nov 2020 01:54:58 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:54:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:55:00 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326a811af266d8284989b860fcf1e92ea12f9c383c5a2b79a622b2096ba7a7`  
		Last Modified: Wed, 28 Oct 2020 18:03:12 GMT  
		Size: 42.0 MB (42029813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d45bc780f2843a5e6d7b59b2552d62db894ec6a13ee501d17d38dfc0046a1`  
		Last Modified: Wed, 28 Oct 2020 18:03:07 GMT  
		Size: 4.1 MB (4063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344e65c3ba5a16c5dd909c6e53eac95b33cc0a725b8742041ab132b8acdc58d7`  
		Last Modified: Tue, 24 Nov 2020 01:59:23 GMT  
		Size: 8.6 KB (8550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d222d1410cf85d1ac39c8864bb3725d32e7cc44f66c2cadd94c1ab7f96538f`  
		Last Modified: Tue, 24 Nov 2020 01:59:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5fbd96f805566c525d74ef696ec238f40b31d37f9c720325b6d642512420d4`  
		Last Modified: Tue, 24 Nov 2020 01:59:29 GMT  
		Size: 173.6 MB (173562229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc5fe6b35b72a7f4f16643e730bdb317016f89873f7b8554303737b8cdeed5f`  
		Last Modified: Tue, 24 Nov 2020 01:59:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b2ef38a3542aac1ccde9752c2ff0bedbaaa290e6bc9c6a4f27412f4b479e34`  
		Last Modified: Tue, 24 Nov 2020 01:59:21 GMT  
		Size: 10.0 KB (10040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2131ce0269b35e413ed535491ce5fbbdd0106e65c99ae0291ed716ae9643cb4`  
		Last Modified: Tue, 24 Nov 2020 01:59:22 GMT  
		Size: 13.0 MB (13000392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.12-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:ff9b703e6b6d99f15e4056508a4bcf4228547fbcf6f89c98fd6f03bc3584b449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.12-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:d8ddf628bcd60d9d7b04037f65ae5f8cfbe4febe36d808be4d48c965dad7b3e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285245204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01dbd22d389e3f49f0bc10ff3d55c22ad57b5149814b2a05c174e3f25e4d359`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:44 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:44 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:34 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:34 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:35 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b301e8e4912399d4efe9baca3d0fbbd6455c25dd47980b4ac4b8fa5cab6441a`  
		Last Modified: Tue, 24 Nov 2020 01:57:40 GMT  
		Size: 8.5 KB (8524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e04408fc6d03bf8ca6dfdebe18d700cae9fc0810e6a7cf6dff9e61d54da906`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3222a371e7cd907495e787f86a28e3afddf26ca48f45553194584f516c4f3df8`  
		Last Modified: Tue, 24 Nov 2020 01:57:50 GMT  
		Size: 173.6 MB (173562178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b79609c22cad5e21937da2fe522e3f795ed5f59c5d6fdf3cbc316ec757ff2`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a601e73fae6400ed40b14573f9e54b61d38ede651d8bf264d5de94d995c7a`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 9.9 KB (9898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362944bb1a2ca37fb1b1dd7ffad50932be48182ee0a67b97ffd3737935ae9cd`  
		Last Modified: Tue, 24 Nov 2020 01:57:41 GMT  
		Size: 13.6 MB (13551482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:e76c103cef8a2a7038801bb40bb9b1b1d64a65b63e4016daa3351b164aa3961b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287704444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2e7bf3831e52ec23bc69904f45ef578bf14c94829832737c97510c22f78b84`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:44:30 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 03:44:33 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:44:35 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 03:44:38 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:44:42 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:44:46 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:44:47 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:44:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:44:50 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:44:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:45:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:45:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:46:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:46:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:47:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:47:23 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:47:28 GMT
USER 1001
# Tue, 24 Nov 2020 03:47:31 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:47:33 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:47:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43c793230c1bc06ea952af86e196c6c84c71921201aeaa9843fbef5ba9df34`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7302a20cb17fd50c657ad3f9830d84023e24495ebe5acea8b01ff028a806b8`  
		Last Modified: Tue, 24 Nov 2020 03:59:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702716097cf974ef7c1ad855c59c86afeda102fb9d42e48ffe786a7a899afb0d`  
		Last Modified: Tue, 24 Nov 2020 03:59:25 GMT  
		Size: 173.6 MB (173562826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b31bcb951bf4e603f2837ada0440f38d229813d9b67118437fca0f5bdd6b58`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f975e52e612075d5916bf563ca11d8ce95982baaa86c8c3e2da13b3fd7e71a`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 10.1 KB (10060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f918938a31f3e45119487cfa30fb1c1402402d8c39c644de919eec00fe597464`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 10.5 MB (10493506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:eed3db11abf068b2f5d23e7cf2c9ef6ca7a1dbb363bf1089d783b095e5d6aaca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280427439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c296a0de601cc1db9da69c6c62c6005dee80ba25360b5a9f2ab076882eb0653`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:58 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:00 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:01 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:01 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:38 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:21 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:21 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:22 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:22 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a94bca6b577989725aa37928cb1e2f8bcb96034452849a0cbb9ffb5009159a`  
		Last Modified: Tue, 24 Nov 2020 01:58:59 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c07fad3f099968bab95bf0189d7f6a3f481c13c5446de9e8f39b839b2da00`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd4714ad37fa09b0664970a83b122b03b4ebf09622a8dde6d0595ffb231b84c`  
		Last Modified: Tue, 24 Nov 2020 01:59:06 GMT  
		Size: 173.6 MB (173562256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac2cdacffdfc4bcd2b78cedaecc6e113a706ee6d44c4111609593f619a50943`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a45c2f182f51e4078348c6ba04cc7c0ec04b7de450c22c8e22bfe1abb3bc12`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 10.0 KB (10045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c01009e4beaff98f2c631248b7783aad02e8a746adf15251bce584e7e0da3c`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 10.6 MB (10584852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.12-kernel-slim-java11-openj9`

```console
$ docker pull open-liberty@sha256:58a82eea77fe13d30c64c58f81a00e67c88f0cbce5e64ec97dfaa761ff6be40b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.12-kernel-slim-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:e3edd79ca3d3091e5fedd25efd89090e91557c860a606e51c9df65cc1936901b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105977814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3179c600ca25676c3079a1a73c36205a3dcc08ec288678323d495e2057c399c9`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:25:27 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:27:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:27:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:27:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:28:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:28:53 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:19 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:19 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:19 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:20 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:20 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:25 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:52:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:52:37 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:52:37 GMT
USER 1001
# Tue, 24 Nov 2020 01:52:37 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:52:38 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:52:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c6ae47f01d1ca61746122b9b904e8cf3d3f16e048774c5c301b535c035c87`  
		Last Modified: Wed, 28 Oct 2020 17:40:51 GMT  
		Size: 42.8 MB (42770675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bffedeca141cd6b2ed75ae8a7aea20289574815afef5089ea410c4305532a8`  
		Last Modified: Wed, 28 Oct 2020 17:40:44 GMT  
		Size: 4.4 MB (4431006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327158e7560add0f2861641f41f1c25dde9b73532cd1dfaa2ea445d7e0d8bb0d`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 8.1 KB (8089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed75dbe28c12eee9dcbec6b8c2ce34686c0a6a4a93998fe00e24d6805b5556`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242b69349c5e71e5f11a28678dbf66dba62690036cbcb2694402a2ffdd858f7f`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 11.6 MB (11638877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068137fcf68e0c921002fde603e80b9cd01d54474fbc02ad78485dcdf67c3061`  
		Last Modified: Tue, 24 Nov 2020 01:57:33 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea350bbbdb66a8b45bcaa35046d6fb107ba3f06b71d6bdefde47b9f4748f7325`  
		Last Modified: Tue, 24 Nov 2020 01:57:33 GMT  
		Size: 9.1 KB (9121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d58b0429d26cfd4bbf27ec76be282e6459bad41460414420e0c26a2e3cd632`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 2.5 MB (2527841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-kernel-slim-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:57830adb4c5f68fcf3e1912e17d9711629df86ff54c80082cea1e9b4a66431cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111674774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c72514207a11557265cd41a6bb813cd792a347e491d090f96379de5c6847f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:29:32 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:32:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:32:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:32:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:34:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:34:21 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:41:52 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:41:59 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 03:42:08 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:42:13 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 03:42:17 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:42:22 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:42:24 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:42:28 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:42:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:42:36 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:42:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:43:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:43:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:43:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:43:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:43:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:43:57 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:44:00 GMT
USER 1001
# Tue, 24 Nov 2020 03:44:03 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:44:07 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:44:10 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9518fb573dc23ad650fc0ea068af5f93f07e910761dbb8b83156f14d391027`  
		Last Modified: Wed, 28 Oct 2020 17:53:00 GMT  
		Size: 43.7 MB (43650458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7e2048088ed2d44960340a046c30cd88499c7356ea5d5da70160cb9286e6de`  
		Last Modified: Wed, 28 Oct 2020 17:52:52 GMT  
		Size: 3.5 MB (3464582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c561600f7fad28df90c2bd991668dc50f67fcaf6b516d5891f44fc5a3f2f7f`  
		Last Modified: Tue, 24 Nov 2020 03:59:00 GMT  
		Size: 8.1 KB (8116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cde82ec9eb0393ea1050e8b546f491cb0d1dec603ead8e6f09511d41b8d7d3`  
		Last Modified: Tue, 24 Nov 2020 03:58:57 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99fbfdb4883bbe55f3e5a1d4ea7ed9eec6aa66abdc17e3a96d1c9908fb7f162`  
		Last Modified: Tue, 24 Nov 2020 03:58:59 GMT  
		Size: 11.6 MB (11639707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de2b5e3f2ec46add6ccb0a98645b0594c2a9eb16469ec329c0c13c2974f9aa9`  
		Last Modified: Tue, 24 Nov 2020 03:58:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d25374215059055ce3498686857628d27bc027d52117f0b4d6eb302eddbbbf`  
		Last Modified: Tue, 24 Nov 2020 03:58:58 GMT  
		Size: 9.2 KB (9240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7929ea9a33fe8690215c31091e4fa73586b715ea9959f4646e57e74dc34ca4bd`  
		Last Modified: Tue, 24 Nov 2020 03:58:57 GMT  
		Size: 2.4 MB (2416607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-kernel-slim-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:f1c1511c79a8b8ce970dfd958b4ecb3b699fb1ab88bfc99a9d6ddd72eabcc77d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103254175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e23871a3ccc0069dfd22542511020041c954d4408f61385483e0f78f95041631`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:47:34 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:49:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:51:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:51:11 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:10 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:11 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:51:11 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:51:12 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:51:13 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:51:14 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:14 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:51:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:51:16 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:51:16 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:51:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:51:28 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:51:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:51:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:51:45 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:51:46 GMT
USER 1001
# Tue, 24 Nov 2020 01:51:46 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:51:47 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:51:48 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326a811af266d8284989b860fcf1e92ea12f9c383c5a2b79a622b2096ba7a7`  
		Last Modified: Wed, 28 Oct 2020 18:03:12 GMT  
		Size: 42.0 MB (42029813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d45bc780f2843a5e6d7b59b2552d62db894ec6a13ee501d17d38dfc0046a1`  
		Last Modified: Wed, 28 Oct 2020 18:03:07 GMT  
		Size: 4.1 MB (4063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98757556e5c82b0a19a8d02431b0bee29a761581c8b760de69684dd4e6ae2ea1`  
		Last Modified: Tue, 24 Nov 2020 01:58:50 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631b6f1b8592750099c773d9ef712641736935d18f41646adee537a399215b1`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8ece28373489c383503dfd5e3056d916307ce3dab6d54ae7d039951a9166f8`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 11.6 MB (11639182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78474d7ee6066218f0f4c52b426b3313862a8be50cdcc4762ddec04da89d6a8e`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e55ac2048927370e1d816cac2fef73d8eec21b0996ae36f601970747d483b7`  
		Last Modified: Tue, 24 Nov 2020 01:58:48 GMT  
		Size: 9.2 KB (9215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3a06e7660289dbcf9b07685ca8271320197e996337eac0441fbbe9e84b197`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 2.5 MB (2504491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.12-kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:76d1836b9e02a305b9aec241f04ff04988e94f36e9c106926adbaff107474cb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.12-kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:5c4ea2b23ff291dcedc3d2e0dbe1981ddbb10d6b448e76c64dced3e268343d97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112314228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06774cf8fdcb304d6c9d722a5a2e484c881893e3aaf1e1c0a0001ae49d9b5ae3`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:51:54 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:54 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:51:54 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:51:54 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:51:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:00 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:52:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:52:11 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:52:11 GMT
USER 1001
# Tue, 24 Nov 2020 01:52:11 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:52:11 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:52:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6b2a07158dbd6daed8528939bab7c0df681b01807294bb012efe4916610631`  
		Last Modified: Tue, 24 Nov 2020 01:57:29 GMT  
		Size: 8.1 KB (8086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485056dec16f9cfe1e0e1d351277068d7d797c3bb09119c34415cde54012288`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782d503069a74c0a09df08b77e8556b46a1549a5dc87a2edc45698519c0b169b`  
		Last Modified: Tue, 24 Nov 2020 01:57:28 GMT  
		Size: 11.6 MB (11638867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b1bf2c650fafa9492af144848a93b789affb748c8b4673543a558ffd6f04`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa51b10b6581890540bed0330311abdc2b6200912c01ef40eb21c4f75ed945d`  
		Last Modified: Tue, 24 Nov 2020 01:57:28 GMT  
		Size: 9.1 KB (9121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e1886c605697fc539432fa97700b746897bdf993d27b5ce1be27d058e631ed`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 2.5 MB (2545356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:7d5949d13ebaaee916360c4987c8c66aea5a3edf5594ac09b89d5e9171491eee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117519089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a1463eb6e194da7f2b5e231f3e9eea0b8dab7b9ebc1509b1aecd1bc420806ba`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:37:54 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 03:38:01 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:38:11 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 03:38:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:38:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:38:32 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:38:39 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:38:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:38:49 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:38:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:39:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:39:37 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:39:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:40:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:40:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:40:58 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:41:14 GMT
USER 1001
# Tue, 24 Nov 2020 03:41:20 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:41:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:41:36 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b05a8d52fa33a6297d98609b8bfcb9026069c0cbdf3da1e15b294e79c8c40f8`  
		Last Modified: Tue, 24 Nov 2020 03:58:43 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64a62e0e109ac620fab4225e3a42fdc95bc5a017d6d1700ed7882e1cee58175`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe321bd61f47be8f42586d917719b52b3be978e7b1de7ac2c39e3cead162061`  
		Last Modified: Tue, 24 Nov 2020 03:58:41 GMT  
		Size: 11.6 MB (11639707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92869bf9ec8109c338682c37e75815a3948b0162780716b990a27eb508fd4574`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed57a01c58b709a379aeed1c95a40b654f3fa1cfb54228e7e04306a9da1708f`  
		Last Modified: Tue, 24 Nov 2020 03:58:41 GMT  
		Size: 9.2 KB (9238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94b7888ef6e8630f2c0a0f0d74b953cd009c74363b0ae78059f70320259d4e8`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 2.2 MB (2232842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.12-kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:3015649ac9dd909f0c06666e2404dda8ae1a3ee0e1191d3df3026732c536ff9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110150274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b050bf871675b24d7d74689a70859e96e79c3c14d5a801ecfa2ba1642d6be6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:50:30 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:50:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:50:32 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:50:32 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:50:33 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:33 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:50:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:50:34 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:50:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:50:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:50:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:50:50 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:51:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:51:01 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:51:01 GMT
USER 1001
# Tue, 24 Nov 2020 01:51:02 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:51:03 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:51:03 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e469be9ecaf59fb92177f742f7178d9a6e001e98998da741eaa7b5acc19c1c1`  
		Last Modified: Tue, 24 Nov 2020 01:58:39 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97086e240c2691f36da8d671679a262c70a61140dfeb0d711c3aee13f05e5baa`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574c871d7727cc1f9ee84fbc31d4414267faa9225d1c3cd11dcfb8d02ce0f50`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 11.6 MB (11639183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280f7d56cfed57c2191fb05d607695894162fc031ef1097ba2f2ee3a4fb5bf5d`  
		Last Modified: Tue, 24 Nov 2020 01:58:33 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60151db569e69bbc6672587ce2c590f5fb465f09a64433b09328d574783ae5e`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 9.2 KB (9220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e599c0bcd50b9ff8283f35bc47725bdc7019228d78ea6cff4b42c08974c0af5`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 2.2 MB (2232341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.9-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:899023df53dfcae9046b186154707c48f619f53453b2fd58758d4686de0f0c57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.9-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:bd271051b97bf1267e6188c0b30afa5e86026fcfb64d332b9913e47d04ce082e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (270016314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e0aa03ffd4e1d4a3d5349ff9619fe2897d1ee56bd9c306eb89b2b46a7f3eac8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_VERSION=20.0.0.9
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_BUILD_LABEL=cl200920200820-0913
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:55:09 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:55:09 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:55:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200920200820-0913 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.9
# Tue, 24 Nov 2020 01:55:09 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:55:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:55:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:55:20 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:55:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:55:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:55:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:55:37 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:55:37 GMT
USER 1001
# Tue, 24 Nov 2020 01:55:37 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:55:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:55:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 24 Nov 2020 01:55:41 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:55:42 GMT
# ARGS: VERBOSE=false
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Tue, 24 Nov 2020 01:56:14 GMT
# ARGS: VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ea815a4bb59bce6ca4ad91229ccc2f10bf230440c8ffabfa9c8d1a192b6f3d`  
		Last Modified: Tue, 24 Nov 2020 01:58:17 GMT  
		Size: 8.5 KB (8519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3a569a7b10d4000e3eaeb1f34455cc032e5046760873b07fcdff3ee9d7e06a`  
		Last Modified: Tue, 24 Nov 2020 01:58:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7201bf433a344c2270022c2426f52cef895a88932f6617bb1041037e5adfac21`  
		Last Modified: Tue, 24 Nov 2020 01:58:25 GMT  
		Size: 158.2 MB (158192088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c238ae6a65e1402667d9a0a7f6c15fb33648d28813c5ea49fb1ff394deea58`  
		Last Modified: Tue, 24 Nov 2020 01:58:15 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7cfa93d9b8ef8c71d6695a6a948bb05a14f3c4a912171cae258efcc4add60`  
		Last Modified: Tue, 24 Nov 2020 01:58:16 GMT  
		Size: 9.6 KB (9571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea10693ba4e84e7b069ee40e4ec012dc734b7fabd88f511efdd197ae95c6f168`  
		Last Modified: Tue, 24 Nov 2020 01:58:16 GMT  
		Size: 4.7 MB (4668802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989fc915562fda1f8f21aee7df6a5e6272f4748f886286e2d4d32bf5a66d86d5`  
		Last Modified: Tue, 24 Nov 2020 01:58:29 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91d0531cf4486d04ae8c2319974301e31cfe4fbc186e79d0ac8fc3f47e38ec2`  
		Last Modified: Tue, 24 Nov 2020 01:58:31 GMT  
		Size: 9.0 MB (9023568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.9-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b12940e7d86e87756cb1a3986bb8daddffbd1a824945197a5ce6c6a7cbfb1a83
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.5 MB (272521454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a99baceef4028ab00cb59b32266c1e4423e357979388fde0b2b2069c97230ce`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:51:32 GMT
ARG LIBERTY_VERSION=20.0.0.9
# Tue, 24 Nov 2020 03:51:39 GMT
ARG LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4
# Tue, 24 Nov 2020 03:51:45 GMT
ARG LIBERTY_BUILD_LABEL=cl200920200820-0913
# Tue, 24 Nov 2020 03:51:53 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip
# Tue, 24 Nov 2020 03:52:05 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:52:15 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:52:25 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:52:31 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:52:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200920200820-0913 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.9
# Tue, 24 Nov 2020 03:52:52 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:52:55 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:54:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:54:39 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:54:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:55:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:55:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:55:38 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:55:41 GMT
USER 1001
# Tue, 24 Nov 2020 03:55:44 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:55:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:55:50 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 24 Nov 2020 03:56:00 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:56:13 GMT
# ARGS: VERBOSE=false
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Tue, 24 Nov 2020 03:57:03 GMT
# ARGS: VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c3560a496034924f4b08aa625f9d892291791c12a7e4d817d7ebecd0716c10`  
		Last Modified: Tue, 24 Nov 2020 04:00:24 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06adf34552dca55f80c60daa76495c6df46dc04518ddb38899ad30a2322c57f2`  
		Last Modified: Tue, 24 Nov 2020 04:00:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9613527c31d36d8f71568b5fab754176c9cfbc8ca68f05550a04001bfec7a117`  
		Last Modified: Tue, 24 Nov 2020 04:00:37 GMT  
		Size: 158.2 MB (158192932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e41f4ed57e50821267e1f4a20407c376c49c5c4285ac9dfddad89ce17a870a`  
		Last Modified: Tue, 24 Nov 2020 04:00:21 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8942c915e8584c856341717b0ed63898dc29a82159e450140289f2e87953a3c8`  
		Last Modified: Tue, 24 Nov 2020 04:00:21 GMT  
		Size: 9.7 KB (9685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf4a7069748e953a5a6bdeaf3f33a495d2166938b584b6e8eb86b3bbe0b35da`  
		Last Modified: Tue, 24 Nov 2020 04:00:21 GMT  
		Size: 3.7 MB (3707253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6943b6051330ff3e00de6b746bf36030f5ad8ac7d486e7c014b709e3372bce`  
		Last Modified: Tue, 24 Nov 2020 04:00:52 GMT  
		Size: 968.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f775b179289950ecb9e637920e2a0f7e06016f2edf0144f0540f7db4ada6548`  
		Last Modified: Tue, 24 Nov 2020 04:00:54 GMT  
		Size: 7.0 MB (6972874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.9-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:8dae54c7f84178d03ba26b9a8195d30c467f85ea5a82b6205d22b93804d6f80f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.2 MB (265219327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7aa84c072fc12d54574c657df2f4ff612860a04ed680ea7fa30f3bc9f42005`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:55:37 GMT
ARG LIBERTY_VERSION=20.0.0.9
# Tue, 24 Nov 2020 01:55:38 GMT
ARG LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4
# Tue, 24 Nov 2020 01:55:38 GMT
ARG LIBERTY_BUILD_LABEL=cl200920200820-0913
# Tue, 24 Nov 2020 01:55:39 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip
# Tue, 24 Nov 2020 01:55:40 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:55:40 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:55:41 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:55:42 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:55:42 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200920200820-0913 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.9
# Tue, 24 Nov 2020 01:55:43 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:55:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:56:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:56:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:56:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:56:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:56:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:56:39 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:56:40 GMT
USER 1001
# Tue, 24 Nov 2020 01:56:40 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:56:41 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:56:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Tue, 24 Nov 2020 01:56:55 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:56:57 GMT
# ARGS: VERBOSE=false
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Tue, 24 Nov 2020 01:57:31 GMT
# ARGS: VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf301a8068c836447555ea5851908df166701103fa7269482b0e0f1434ec685`  
		Last Modified: Tue, 24 Nov 2020 01:59:48 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c3415643bab4e202885093c6a2734af67ea744355281cf19f080735ccfe490`  
		Last Modified: Tue, 24 Nov 2020 01:59:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689848d049e904e825e2494090ad8331a944bd0bafea3c74da0543caf5536587`  
		Last Modified: Tue, 24 Nov 2020 01:59:53 GMT  
		Size: 158.2 MB (158192393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3e7253714e36daf77292c773f70447266555f1d25847e24c69d335c83424ee`  
		Last Modified: Tue, 24 Nov 2020 01:59:46 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21b4ccaa0ed5801e9a162156b053909ffbb6c1577a0b43d6498fea564ca9a7`  
		Last Modified: Tue, 24 Nov 2020 01:59:46 GMT  
		Size: 9.7 KB (9657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f10673696eda4b429e8279bdcff24f075f694094b8da1a29d9b072bf29dfbe`  
		Last Modified: Tue, 24 Nov 2020 01:59:46 GMT  
		Size: 3.7 MB (3736745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a62a3985dd75b9e752cbb0b590b0fa644e994ccfd3f7dc17ed7938185c34ab0`  
		Last Modified: Tue, 24 Nov 2020 02:00:04 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38178f10f5ae3b82b856e5e73764494eee5434e375f29dcaa88ebedcdf2f0d14`  
		Last Modified: Tue, 24 Nov 2020 02:00:04 GMT  
		Size: 7.0 MB (7009611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.9-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:668ffb514e581e7f73ae8343d9a0bdce7932e67178505c2406938f65299d2db8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.9-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:bc6f10aafe7a46d186b900d83b62e488a2efb45337e64b5617a76bdf2ff06a26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (260991780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039b4c132d4980eec088ac74cae8ce0137418b84e257aa5e6cc0977542e5fd7c`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_VERSION=20.0.0.9
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_BUILD_LABEL=cl200920200820-0913
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:55:08 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:55:09 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:55:09 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:55:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200920200820-0913 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.9
# Tue, 24 Nov 2020 01:55:09 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:55:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:55:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:55:20 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:55:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:55:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:55:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:55:37 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:55:37 GMT
USER 1001
# Tue, 24 Nov 2020 01:55:37 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:55:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:55:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ea815a4bb59bce6ca4ad91229ccc2f10bf230440c8ffabfa9c8d1a192b6f3d`  
		Last Modified: Tue, 24 Nov 2020 01:58:17 GMT  
		Size: 8.5 KB (8519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3a569a7b10d4000e3eaeb1f34455cc032e5046760873b07fcdff3ee9d7e06a`  
		Last Modified: Tue, 24 Nov 2020 01:58:15 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7201bf433a344c2270022c2426f52cef895a88932f6617bb1041037e5adfac21`  
		Last Modified: Tue, 24 Nov 2020 01:58:25 GMT  
		Size: 158.2 MB (158192088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c238ae6a65e1402667d9a0a7f6c15fb33648d28813c5ea49fb1ff394deea58`  
		Last Modified: Tue, 24 Nov 2020 01:58:15 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7cfa93d9b8ef8c71d6695a6a948bb05a14f3c4a912171cae258efcc4add60`  
		Last Modified: Tue, 24 Nov 2020 01:58:16 GMT  
		Size: 9.6 KB (9571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea10693ba4e84e7b069ee40e4ec012dc734b7fabd88f511efdd197ae95c6f168`  
		Last Modified: Tue, 24 Nov 2020 01:58:16 GMT  
		Size: 4.7 MB (4668802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.9-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:625f3ec9e84073e788f1360ce9be2fe7fba1c766189dd002ec02ffb4e64d37c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.5 MB (265547612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0a754c08aabef962e71af32b64072e45672beb6d2f10c619696f68012635c8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:51:32 GMT
ARG LIBERTY_VERSION=20.0.0.9
# Tue, 24 Nov 2020 03:51:39 GMT
ARG LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4
# Tue, 24 Nov 2020 03:51:45 GMT
ARG LIBERTY_BUILD_LABEL=cl200920200820-0913
# Tue, 24 Nov 2020 03:51:53 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip
# Tue, 24 Nov 2020 03:52:05 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:52:15 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:52:25 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:52:31 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:52:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200920200820-0913 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.9
# Tue, 24 Nov 2020 03:52:52 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:52:55 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:54:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:54:39 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:54:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:55:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:55:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:55:38 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:55:41 GMT
USER 1001
# Tue, 24 Nov 2020 03:55:44 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:55:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:55:50 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c3560a496034924f4b08aa625f9d892291791c12a7e4d817d7ebecd0716c10`  
		Last Modified: Tue, 24 Nov 2020 04:00:24 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06adf34552dca55f80c60daa76495c6df46dc04518ddb38899ad30a2322c57f2`  
		Last Modified: Tue, 24 Nov 2020 04:00:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9613527c31d36d8f71568b5fab754176c9cfbc8ca68f05550a04001bfec7a117`  
		Last Modified: Tue, 24 Nov 2020 04:00:37 GMT  
		Size: 158.2 MB (158192932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e41f4ed57e50821267e1f4a20407c376c49c5c4285ac9dfddad89ce17a870a`  
		Last Modified: Tue, 24 Nov 2020 04:00:21 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8942c915e8584c856341717b0ed63898dc29a82159e450140289f2e87953a3c8`  
		Last Modified: Tue, 24 Nov 2020 04:00:21 GMT  
		Size: 9.7 KB (9685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf4a7069748e953a5a6bdeaf3f33a495d2166938b584b6e8eb86b3bbe0b35da`  
		Last Modified: Tue, 24 Nov 2020 04:00:21 GMT  
		Size: 3.7 MB (3707253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.9-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:b25e81c0c9a05532ad1f4eb5274e02ec6fb8b142581fb852fc13ad0b7429fbf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.2 MB (258208751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ccd500d73923c010b27472f285a86dbfd4090b5891c04c2d986640822dbb3b`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:55:37 GMT
ARG LIBERTY_VERSION=20.0.0.9
# Tue, 24 Nov 2020 01:55:38 GMT
ARG LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4
# Tue, 24 Nov 2020 01:55:38 GMT
ARG LIBERTY_BUILD_LABEL=cl200920200820-0913
# Tue, 24 Nov 2020 01:55:39 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip
# Tue, 24 Nov 2020 01:55:40 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:55:40 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:55:41 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:55:42 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:55:42 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200920200820-0913 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.9
# Tue, 24 Nov 2020 01:55:43 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:55:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:56:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:56:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:56:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:56:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:56:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200920200820-0913 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.9/openliberty-runtime-20.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=c354fd0e0d3704cc63d4f0810e38f5d081916ef4 LIBERTY_VERSION=20.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:56:39 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:56:40 GMT
USER 1001
# Tue, 24 Nov 2020 01:56:40 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:56:41 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:56:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf301a8068c836447555ea5851908df166701103fa7269482b0e0f1434ec685`  
		Last Modified: Tue, 24 Nov 2020 01:59:48 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c3415643bab4e202885093c6a2734af67ea744355281cf19f080735ccfe490`  
		Last Modified: Tue, 24 Nov 2020 01:59:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689848d049e904e825e2494090ad8331a944bd0bafea3c74da0543caf5536587`  
		Last Modified: Tue, 24 Nov 2020 01:59:53 GMT  
		Size: 158.2 MB (158192393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3e7253714e36daf77292c773f70447266555f1d25847e24c69d335c83424ee`  
		Last Modified: Tue, 24 Nov 2020 01:59:46 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c21b4ccaa0ed5801e9a162156b053909ffbb6c1577a0b43d6498fea564ca9a7`  
		Last Modified: Tue, 24 Nov 2020 01:59:46 GMT  
		Size: 9.7 KB (9657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f10673696eda4b429e8279bdcff24f075f694094b8da1a29d9b072bf29dfbe`  
		Last Modified: Tue, 24 Nov 2020 01:59:46 GMT  
		Size: 3.7 MB (3736745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.1-full-java11-openj9`

**does not exist** (yet?)

## `open-liberty:21.0.0.1-full-java8-openj9`

**does not exist** (yet?)

## `open-liberty:21.0.0.1-kernel-slim-java11-openj9`

**does not exist** (yet?)

## `open-liberty:21.0.0.1-kernel-slim-java8-openj9`

**does not exist** (yet?)

## `open-liberty:beta`

```console
$ docker pull open-liberty@sha256:25dad70a8eceadf31d0b6d0ccb97707d119e92232f923d762c846de4c3b23826
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta` - linux; amd64

```console
$ docker pull open-liberty@sha256:22a93b513efe42495d52a2114b1cb2071714678faa2e385936565300b1321da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.2 MB (336154232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb949b9c5677fa407104a6ccf3eb26b4ac28f06eef5890b1baaf3fbb98c189a0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:49:40 GMT
ARG LIBERTY_VERSION=21.0.0.1
# Tue, 24 Nov 2020 01:49:40 GMT
ARG LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335
# Tue, 24 Nov 2020 01:49:40 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:49:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip
# Tue, 24 Nov 2020 01:49:41 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:49:41 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:49:41 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:49:41 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:49:41 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with AdoptOpenJDK 8 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=21.0.0.1
# Tue, 24 Nov 2020 01:49:42 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:49:42 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:49:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:49:55 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:49:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:49:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:50:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:50:39 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:50:39 GMT
USER 1001
# Tue, 24 Nov 2020 01:50:39 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:50:39 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:50:40 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0057385b6709b06d72fd5ccae5d1cdb36e865f7cd7a5be892833e11f809a911b`  
		Last Modified: Tue, 24 Nov 2020 01:56:30 GMT  
		Size: 8.5 KB (8517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a97c16cb8ed7046316a44eed530407e4526b6ee678191fca98548e8ee0cf32a`  
		Last Modified: Tue, 24 Nov 2020 01:56:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c09de95d379d5a444fdb87215b5f95e741c33d7c2797bfbba37dbc3a9c62c`  
		Last Modified: Tue, 24 Nov 2020 01:56:45 GMT  
		Size: 224.6 MB (224636347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d6ad049a84976bc8d24fa15a13c6d37793f4124e8564971be0e2a773cbb00`  
		Last Modified: Tue, 24 Nov 2020 01:56:29 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ed4f0f6d6ca9aeec982899457777067e673596cf57563b888229de4678a4d5`  
		Last Modified: Tue, 24 Nov 2020 01:56:30 GMT  
		Size: 9.9 KB (9900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e89da7c7796e042c746502d1d6ddbc7a399ef5d933dac6f62bb1e4152c08d6a`  
		Last Modified: Tue, 24 Nov 2020 01:56:32 GMT  
		Size: 13.4 MB (13386350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:900903bcfe4d124dd73f6acdf84ce143c3f677a44794bc4c30d53a5732ac48aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.8 MB (338795302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da0a7dec0398ce73385f2fdfc4829edc8e87a7b4b37d62df8f38f015e782659`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:29:01 GMT
ARG LIBERTY_VERSION=21.0.0.1
# Tue, 24 Nov 2020 03:29:10 GMT
ARG LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335
# Tue, 24 Nov 2020 03:29:17 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:29:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip
# Tue, 24 Nov 2020 03:29:28 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:29:34 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:29:38 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:29:43 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:29:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with AdoptOpenJDK 8 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=21.0.0.1
# Tue, 24 Nov 2020 03:29:51 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:29:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:30:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:30:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:31:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:31:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:32:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:32:32 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:32:35 GMT
USER 1001
# Tue, 24 Nov 2020 03:32:37 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:32:41 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:32:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e19e6153436432ff249ca53d232839efad365d8286d0c226acedbf1614121`  
		Last Modified: Tue, 24 Nov 2020 03:57:32 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2e8d64ed6095db424798c4fab239ba8f870ee70b0bcbea4623e168b6910189`  
		Last Modified: Tue, 24 Nov 2020 03:57:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fb6c7d66112db2f01ed406c7a9dd50e69f73e30eb305371bec487534eb002c`  
		Last Modified: Tue, 24 Nov 2020 03:57:54 GMT  
		Size: 224.6 MB (224637205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e077ac5d3476a328056791d3f0461fa4b7ba81cf65043067176652b851c53ab`  
		Last Modified: Tue, 24 Nov 2020 03:57:29 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b3c581e6e34af4baa398fb160a4c030680cbea878d0b43e048c9beabdb96f`  
		Last Modified: Tue, 24 Nov 2020 03:57:29 GMT  
		Size: 10.1 KB (10078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337068db25f0f617d89f4a6389e4cac12a2ebea776957b58c115ad0e89e6de7b`  
		Last Modified: Tue, 24 Nov 2020 03:57:31 GMT  
		Size: 10.5 MB (10509954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta` - linux; s390x

```console
$ docker pull open-liberty@sha256:da19488b47961f2b2c5197305ba4ee74ef3b8a275d79f9ecf8d646e3d7ebdc07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331519636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957446c96ecf3592be53b558ae9b69f41f8e082eab2def6e5632749f264c0245`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:46:52 GMT
ARG LIBERTY_VERSION=21.0.0.1
# Tue, 24 Nov 2020 01:46:53 GMT
ARG LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335
# Tue, 24 Nov 2020 01:46:53 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:46:54 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip
# Tue, 24 Nov 2020 01:46:54 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:46:55 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:46:56 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:46:56 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:46:57 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with AdoptOpenJDK 8 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=21.0.0.1
# Tue, 24 Nov 2020 01:46:57 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:46:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:47:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:47:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:47:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:47:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:48:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:48:30 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:48:30 GMT
USER 1001
# Tue, 24 Nov 2020 01:48:31 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:48:32 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:48:32 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967f3498412140d55086237bf871e4c6a9ecd21fb1e53e8c6936e21d78a032b`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a15174cf0ce26e12c4071f42945e9a0c47ff8c06f4db6804f43d927cdf5cc0a`  
		Last Modified: Tue, 24 Nov 2020 01:57:55 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76b0ae441db493b356ce23f5ffbc805700ebbc8cddf883cb5295caa001b3b`  
		Last Modified: Tue, 24 Nov 2020 01:58:06 GMT  
		Size: 224.6 MB (224636687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86442d91adf4e6b0a62d8e9af47b2b7c180f50d7a32f8b8ef637d000ca52514d`  
		Last Modified: Tue, 24 Nov 2020 01:57:56 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cec3dd9fee38f5a9e21189b5fd0cee0d6a4e32e94f086ca82d0cbe8cd43f664`  
		Last Modified: Tue, 24 Nov 2020 01:57:55 GMT  
		Size: 10.1 KB (10058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33bcaeee4521a2021395f312be56fb7247c09cf01bbe9bf7aae843f604beeb4`  
		Last Modified: Tue, 24 Nov 2020 01:57:59 GMT  
		Size: 10.6 MB (10602604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:beta-java11`

```console
$ docker pull open-liberty@sha256:f45e3acca8a68375b7969a837979e19a074dcd16f96419b350093a9949cd35f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta-java11` - linux; amd64

```console
$ docker pull open-liberty@sha256:8122c552164e0070e28765b67d4cb4db8be5c7e401ebb2015141e9d2ae21020c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.2 MB (330242970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772d7ef025c60d5c793188a249db20ae91f5c43f2fc7497ad237498b1f9383fb`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:25:27 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:27:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:27:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:27:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:28:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:28:53 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:46 GMT
ARG LIBERTY_VERSION=21.0.0.1
# Tue, 24 Nov 2020 01:50:46 GMT
ARG LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335
# Tue, 24 Nov 2020 01:50:47 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:50:47 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip
# Tue, 24 Nov 2020 01:50:47 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:50:47 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:50:47 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:48 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:50:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with AdoptOpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=21.0.0.1
# Tue, 24 Nov 2020 01:50:48 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:50:48 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:51:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:51:02 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:51:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:51:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:51:46 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:51:46 GMT
USER 1001
# Tue, 24 Nov 2020 01:51:46 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:51:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:51:46 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c6ae47f01d1ca61746122b9b904e8cf3d3f16e048774c5c301b535c035c87`  
		Last Modified: Wed, 28 Oct 2020 17:40:51 GMT  
		Size: 42.8 MB (42770675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bffedeca141cd6b2ed75ae8a7aea20289574815afef5089ea410c4305532a8`  
		Last Modified: Wed, 28 Oct 2020 17:40:44 GMT  
		Size: 4.4 MB (4431006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228bc06574eff61197fbc2fea7a3c5d80ac8ae9b20019409d976ee9ed6d7ad5d`  
		Last Modified: Tue, 24 Nov 2020 01:56:52 GMT  
		Size: 8.5 KB (8517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8805643561eb0bbbcbdbff4a10496b611350fd1c5f1033712407d3fdf18ba1a7`  
		Last Modified: Tue, 24 Nov 2020 01:56:51 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152c8967e8a66f5a27ce960aab03e5d7a97359a91cdbf20a3f7864df18a28f89`  
		Last Modified: Tue, 24 Nov 2020 01:57:23 GMT  
		Size: 224.6 MB (224636359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbf4d3fc403ad8a0bcd668f2f9c8e41b2565eff088b6d334f049025a40741`  
		Last Modified: Tue, 24 Nov 2020 01:56:50 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b324e37a571036d2721537aa236fa5a54862e70e8c8ff14e30e362c6298187`  
		Last Modified: Tue, 24 Nov 2020 01:56:51 GMT  
		Size: 9.9 KB (9896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04147bcf59ab686e0639608ad3df79cbba914c03b17f6b46225a275c67b3bb0d`  
		Last Modified: Tue, 24 Nov 2020 01:56:54 GMT  
		Size: 13.8 MB (13793995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:6e8cb353b4bd52a1d0c2046d50dc44f01e50f575ec13897df735ba483b0f93e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334149442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0691a714ce3db560dcc16bbfb1d07d002ecea3fa09e314724a8a56bd0730a61a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:29:32 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:32:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:32:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:32:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:34:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:34:21 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:32:53 GMT
ARG LIBERTY_VERSION=21.0.0.1
# Tue, 24 Nov 2020 03:32:59 GMT
ARG LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335
# Tue, 24 Nov 2020 03:33:02 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:33:08 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip
# Tue, 24 Nov 2020 03:33:12 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:33:21 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:33:41 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:33:55 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:34:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with AdoptOpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=21.0.0.1
# Tue, 24 Nov 2020 03:34:17 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:34:20 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:35:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:35:17 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:35:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:35:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:37:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:37:11 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:37:17 GMT
USER 1001
# Tue, 24 Nov 2020 03:37:20 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:37:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:37:34 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9518fb573dc23ad650fc0ea068af5f93f07e910761dbb8b83156f14d391027`  
		Last Modified: Wed, 28 Oct 2020 17:53:00 GMT  
		Size: 43.7 MB (43650458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7e2048088ed2d44960340a046c30cd88499c7356ea5d5da70160cb9286e6de`  
		Last Modified: Wed, 28 Oct 2020 17:52:52 GMT  
		Size: 3.5 MB (3464582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d15ec7dde9cc7407cdc894f195384059fa862dcbf6583c1e1ed9ab0bcf71f3`  
		Last Modified: Tue, 24 Nov 2020 03:58:11 GMT  
		Size: 8.6 KB (8550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fdf298c4242984362a1f5244f0bd56467d1221644932566056b24416f708fc`  
		Last Modified: Tue, 24 Nov 2020 03:58:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b382b000291b2eb9fa74956484e09adb029b06ec26ff7c85da18d1ec313ec`  
		Last Modified: Tue, 24 Nov 2020 03:58:30 GMT  
		Size: 224.6 MB (224637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e396a996398cdb0e991b39fee1cf988910fe7c7428b8e01ebe114bed0f34c1`  
		Last Modified: Tue, 24 Nov 2020 03:58:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a304acd31c5575ac69337c1deb3009825f1602fa40ee3b4f15bacbe5d187550`  
		Last Modified: Tue, 24 Nov 2020 03:58:08 GMT  
		Size: 10.1 KB (10069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d798d8af5e910b596ebc2a8add146e57561bcfd05beae198e75ae8679cbe90`  
		Last Modified: Tue, 24 Nov 2020 03:58:11 GMT  
		Size: 11.9 MB (11892158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; s390x

```console
$ docker pull open-liberty@sha256:6c78b0ff1e7eb18e53bb1095e6410766a9ef88660926ce879128998ebac12479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326842912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b791dcf33cc6048606a35371c8a583dfac414379f46c43d1036620c41a642244`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:47:34 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:49:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:51:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:51:11 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:48:40 GMT
ARG LIBERTY_VERSION=21.0.0.1
# Tue, 24 Nov 2020 01:48:41 GMT
ARG LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335
# Tue, 24 Nov 2020 01:48:41 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:48:42 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip
# Tue, 24 Nov 2020 01:48:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:48:43 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:48:43 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:48:44 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:48:45 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with AdoptOpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=21.0.0.1
# Tue, 24 Nov 2020 01:48:45 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:48:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:49:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:49:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:49:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:49:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:50:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/21.0.0.1-beta/openliberty-runtime-21.0.0.1-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=5abe9cb23bc2f9ab2443699dd502b41bdca13335 LIBERTY_VERSION=21.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:50:14 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:50:14 GMT
USER 1001
# Tue, 24 Nov 2020 01:50:15 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:50:15 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:50:16 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326a811af266d8284989b860fcf1e92ea12f9c383c5a2b79a622b2096ba7a7`  
		Last Modified: Wed, 28 Oct 2020 18:03:12 GMT  
		Size: 42.0 MB (42029813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d45bc780f2843a5e6d7b59b2552d62db894ec6a13ee501d17d38dfc0046a1`  
		Last Modified: Wed, 28 Oct 2020 18:03:07 GMT  
		Size: 4.1 MB (4063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f174a4677cc603a07cac64c54ae980bf931281bda78f1accca781dd130308`  
		Last Modified: Tue, 24 Nov 2020 01:58:16 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388a5319f4dfa1017210c1371289dd5a1800a4f3e51e3a057df20e3a7c1b196`  
		Last Modified: Tue, 24 Nov 2020 01:58:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c5796cb0beba79f323892b1501a8c0988de5344165cadc0b5ec303f90fc528`  
		Last Modified: Tue, 24 Nov 2020 01:58:26 GMT  
		Size: 224.6 MB (224636705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f12c4b5f8be65cb45e55c8005c27a56dac2d1c78c517ad07146decd17ee77e`  
		Last Modified: Tue, 24 Nov 2020 01:58:13 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c326cb7894f8349b401e882918bac86d1938e47dbcceef5c84a0918be014b2`  
		Last Modified: Tue, 24 Nov 2020 01:58:13 GMT  
		Size: 10.1 KB (10053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcca5ce2f44b98b758de03a82ccba7e38c4d6e9180f040bb4b17f47e4db69477`  
		Last Modified: Tue, 24 Nov 2020 01:58:16 GMT  
		Size: 13.1 MB (13094109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:ff9b703e6b6d99f15e4056508a4bcf4228547fbcf6f89c98fd6f03bc3584b449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:d8ddf628bcd60d9d7b04037f65ae5f8cfbe4febe36d808be4d48c965dad7b3e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285245204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01dbd22d389e3f49f0bc10ff3d55c22ad57b5149814b2a05c174e3f25e4d359`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:44 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:44 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:34 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:34 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:35 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b301e8e4912399d4efe9baca3d0fbbd6455c25dd47980b4ac4b8fa5cab6441a`  
		Last Modified: Tue, 24 Nov 2020 01:57:40 GMT  
		Size: 8.5 KB (8524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e04408fc6d03bf8ca6dfdebe18d700cae9fc0810e6a7cf6dff9e61d54da906`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3222a371e7cd907495e787f86a28e3afddf26ca48f45553194584f516c4f3df8`  
		Last Modified: Tue, 24 Nov 2020 01:57:50 GMT  
		Size: 173.6 MB (173562178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b79609c22cad5e21937da2fe522e3f795ed5f59c5d6fdf3cbc316ec757ff2`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a601e73fae6400ed40b14573f9e54b61d38ede651d8bf264d5de94d995c7a`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 9.9 KB (9898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362944bb1a2ca37fb1b1dd7ffad50932be48182ee0a67b97ffd3737935ae9cd`  
		Last Modified: Tue, 24 Nov 2020 01:57:41 GMT  
		Size: 13.6 MB (13551482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:e76c103cef8a2a7038801bb40bb9b1b1d64a65b63e4016daa3351b164aa3961b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287704444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2e7bf3831e52ec23bc69904f45ef578bf14c94829832737c97510c22f78b84`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:44:30 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 03:44:33 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:44:35 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 03:44:38 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:44:42 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:44:46 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:44:47 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:44:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:44:50 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:44:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:45:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:45:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:46:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:46:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:47:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:47:23 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:47:28 GMT
USER 1001
# Tue, 24 Nov 2020 03:47:31 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:47:33 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:47:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43c793230c1bc06ea952af86e196c6c84c71921201aeaa9843fbef5ba9df34`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7302a20cb17fd50c657ad3f9830d84023e24495ebe5acea8b01ff028a806b8`  
		Last Modified: Tue, 24 Nov 2020 03:59:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702716097cf974ef7c1ad855c59c86afeda102fb9d42e48ffe786a7a899afb0d`  
		Last Modified: Tue, 24 Nov 2020 03:59:25 GMT  
		Size: 173.6 MB (173562826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b31bcb951bf4e603f2837ada0440f38d229813d9b67118437fca0f5bdd6b58`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f975e52e612075d5916bf563ca11d8ce95982baaa86c8c3e2da13b3fd7e71a`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 10.1 KB (10060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f918938a31f3e45119487cfa30fb1c1402402d8c39c644de919eec00fe597464`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 10.5 MB (10493506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:eed3db11abf068b2f5d23e7cf2c9ef6ca7a1dbb363bf1089d783b095e5d6aaca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280427439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c296a0de601cc1db9da69c6c62c6005dee80ba25360b5a9f2ab076882eb0653`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:58 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:00 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:01 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:01 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:38 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:21 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:21 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:22 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:22 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a94bca6b577989725aa37928cb1e2f8bcb96034452849a0cbb9ffb5009159a`  
		Last Modified: Tue, 24 Nov 2020 01:58:59 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c07fad3f099968bab95bf0189d7f6a3f481c13c5446de9e8f39b839b2da00`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd4714ad37fa09b0664970a83b122b03b4ebf09622a8dde6d0595ffb231b84c`  
		Last Modified: Tue, 24 Nov 2020 01:59:06 GMT  
		Size: 173.6 MB (173562256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac2cdacffdfc4bcd2b78cedaecc6e113a706ee6d44c4111609593f619a50943`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a45c2f182f51e4078348c6ba04cc7c0ec04b7de450c22c8e22bfe1abb3bc12`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 10.0 KB (10045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c01009e4beaff98f2c631248b7783aad02e8a746adf15251bce584e7e0da3c`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 10.6 MB (10584852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java11-openj9`

```console
$ docker pull open-liberty@sha256:c890cc586507f0f7979252cca708dc50554ff9fd656b152c4eda949998a2016c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:8ac167d3164315d4fd74bef7d9122c3532f42544ed0957056825eb49aa5cf6ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.2 MB (279171024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca444551af85dd00b08e3cfc5fea00b3c589831ac2e4369aa4f839c1f7a282a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:25:27 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:27:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:27:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:27:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:28:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:28:53 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:53:48 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:53:49 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:53:49 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:53:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:53:49 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:53:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:54:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:54:01 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:54:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:54:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:54:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:54:42 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:54:43 GMT
USER 1001
# Tue, 24 Nov 2020 01:54:43 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:54:43 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:54:43 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c6ae47f01d1ca61746122b9b904e8cf3d3f16e048774c5c301b535c035c87`  
		Last Modified: Wed, 28 Oct 2020 17:40:51 GMT  
		Size: 42.8 MB (42770675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bffedeca141cd6b2ed75ae8a7aea20289574815afef5089ea410c4305532a8`  
		Last Modified: Wed, 28 Oct 2020 17:40:44 GMT  
		Size: 4.4 MB (4431006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26960407c3776c8b5df4a9fbf761863b267bef198b4fce4f1ef2bc52ab4a0980`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 8.5 KB (8516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e929c87ce24fca4109057fadaf4288c2fec5fa8189f17894b1aa512ea9095776`  
		Last Modified: Tue, 24 Nov 2020 01:57:56 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830cb5582179b38d8d635e7d9596337d35fe6bf586f1079eb6a48f7ce8a3b0bd`  
		Last Modified: Tue, 24 Nov 2020 01:58:07 GMT  
		Size: 173.6 MB (173562103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9acb0edaf613f391a8ea09d433c0257d011381b422f23886f5c9840c5865a1`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037abc0895b48f5936b240d870104a8720c29d0cd9eb9a27c614ab1643d026b6`  
		Last Modified: Tue, 24 Nov 2020 01:57:57 GMT  
		Size: 9.9 KB (9900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9db8da445ba07b490b0394018ad9883786e4b1047f183caabc203fb2b0208b`  
		Last Modified: Tue, 24 Nov 2020 01:57:59 GMT  
		Size: 13.8 MB (13796295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:ad5f1845f680d430a69059362583d8cf15e5a40857c7705624d1d46e38dc7117
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.2 MB (283191950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:416dbec692ae7e5086385a69fbff91be75a5ed94c45dbe91e83029b74344c2ce`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:29:32 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:32:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:32:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:32:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:34:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:34:21 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:41:52 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:47:55 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 03:48:00 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:48:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 03:48:07 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:48:09 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:48:13 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:48:16 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:48:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:48:20 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:48:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:48:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:48:58 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:49:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:49:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:50:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:50:50 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:50:53 GMT
USER 1001
# Tue, 24 Nov 2020 03:50:57 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:51:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:51:10 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9518fb573dc23ad650fc0ea068af5f93f07e910761dbb8b83156f14d391027`  
		Last Modified: Wed, 28 Oct 2020 17:53:00 GMT  
		Size: 43.7 MB (43650458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7e2048088ed2d44960340a046c30cd88499c7356ea5d5da70160cb9286e6de`  
		Last Modified: Wed, 28 Oct 2020 17:52:52 GMT  
		Size: 3.5 MB (3464582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ca5f33c45bc1fb66d815593bed20c1fa116c2577117135a535b975e6d0669a`  
		Last Modified: Tue, 24 Nov 2020 03:59:45 GMT  
		Size: 8.5 KB (8549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c5b1d0f1062df749fafac658321c6e09b301a3bb5b4d2d353ba2e721fbb421`  
		Last Modified: Tue, 24 Nov 2020 03:59:41 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7066a36d28eb4dc8face0f1d38076e2d893d57d601a1ae4cc766f838b906d6a`  
		Last Modified: Tue, 24 Nov 2020 03:59:59 GMT  
		Size: 173.6 MB (173562818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fb888ec1de655aefa72caec26571dc95f30b98e5b733523bf02966728c8295`  
		Last Modified: Tue, 24 Nov 2020 03:59:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca8149a48aaf46787b9df7436786ec7c870640634a3947a72dd4e0c6b619af`  
		Last Modified: Tue, 24 Nov 2020 03:59:42 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b939e34871786a62e214174d2588eef1dbda71eb753de5aae93a05048e64d6`  
		Last Modified: Tue, 24 Nov 2020 03:59:46 GMT  
		Size: 12.0 MB (12009096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:cf8858f9efaa44ced868f90cd690c36f386073702faeff5ac20268392b385d55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.7 MB (275674712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82702e38a99d995b87e8195a1b9f3bce7c6281033b881d6bffbb7bc29cff87a0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:47:34 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:49:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:51:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:51:11 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:10 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:53:31 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:53:32 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:53:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:53:33 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:53:34 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:53:34 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:53:35 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:53:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:53:36 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:53:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:54:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:54:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:54:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:54:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:54:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:54:57 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:54:58 GMT
USER 1001
# Tue, 24 Nov 2020 01:54:58 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:54:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:55:00 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326a811af266d8284989b860fcf1e92ea12f9c383c5a2b79a622b2096ba7a7`  
		Last Modified: Wed, 28 Oct 2020 18:03:12 GMT  
		Size: 42.0 MB (42029813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d45bc780f2843a5e6d7b59b2552d62db894ec6a13ee501d17d38dfc0046a1`  
		Last Modified: Wed, 28 Oct 2020 18:03:07 GMT  
		Size: 4.1 MB (4063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344e65c3ba5a16c5dd909c6e53eac95b33cc0a725b8742041ab132b8acdc58d7`  
		Last Modified: Tue, 24 Nov 2020 01:59:23 GMT  
		Size: 8.6 KB (8550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d222d1410cf85d1ac39c8864bb3725d32e7cc44f66c2cadd94c1ab7f96538f`  
		Last Modified: Tue, 24 Nov 2020 01:59:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5fbd96f805566c525d74ef696ec238f40b31d37f9c720325b6d642512420d4`  
		Last Modified: Tue, 24 Nov 2020 01:59:29 GMT  
		Size: 173.6 MB (173562229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc5fe6b35b72a7f4f16643e730bdb317016f89873f7b8554303737b8cdeed5f`  
		Last Modified: Tue, 24 Nov 2020 01:59:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b2ef38a3542aac1ccde9752c2ff0bedbaaa290e6bc9c6a4f27412f4b479e34`  
		Last Modified: Tue, 24 Nov 2020 01:59:21 GMT  
		Size: 10.0 KB (10040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2131ce0269b35e413ed535491ce5fbbdd0106e65c99ae0291ed716ae9643cb4`  
		Last Modified: Tue, 24 Nov 2020 01:59:22 GMT  
		Size: 13.0 MB (13000392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java8-openj9`

```console
$ docker pull open-liberty@sha256:ff9b703e6b6d99f15e4056508a4bcf4228547fbcf6f89c98fd6f03bc3584b449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:d8ddf628bcd60d9d7b04037f65ae5f8cfbe4febe36d808be4d48c965dad7b3e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285245204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01dbd22d389e3f49f0bc10ff3d55c22ad57b5149814b2a05c174e3f25e4d359`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:44 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:44 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:34 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:34 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:35 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b301e8e4912399d4efe9baca3d0fbbd6455c25dd47980b4ac4b8fa5cab6441a`  
		Last Modified: Tue, 24 Nov 2020 01:57:40 GMT  
		Size: 8.5 KB (8524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e04408fc6d03bf8ca6dfdebe18d700cae9fc0810e6a7cf6dff9e61d54da906`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3222a371e7cd907495e787f86a28e3afddf26ca48f45553194584f516c4f3df8`  
		Last Modified: Tue, 24 Nov 2020 01:57:50 GMT  
		Size: 173.6 MB (173562178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b79609c22cad5e21937da2fe522e3f795ed5f59c5d6fdf3cbc316ec757ff2`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a601e73fae6400ed40b14573f9e54b61d38ede651d8bf264d5de94d995c7a`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 9.9 KB (9898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362944bb1a2ca37fb1b1dd7ffad50932be48182ee0a67b97ffd3737935ae9cd`  
		Last Modified: Tue, 24 Nov 2020 01:57:41 GMT  
		Size: 13.6 MB (13551482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:e76c103cef8a2a7038801bb40bb9b1b1d64a65b63e4016daa3351b164aa3961b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287704444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2e7bf3831e52ec23bc69904f45ef578bf14c94829832737c97510c22f78b84`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:44:30 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 03:44:33 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:44:35 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 03:44:38 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:44:42 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:44:46 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:44:47 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:44:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:44:50 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:44:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:45:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:45:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:46:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:46:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:47:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:47:23 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:47:28 GMT
USER 1001
# Tue, 24 Nov 2020 03:47:31 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:47:33 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:47:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43c793230c1bc06ea952af86e196c6c84c71921201aeaa9843fbef5ba9df34`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7302a20cb17fd50c657ad3f9830d84023e24495ebe5acea8b01ff028a806b8`  
		Last Modified: Tue, 24 Nov 2020 03:59:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702716097cf974ef7c1ad855c59c86afeda102fb9d42e48ffe786a7a899afb0d`  
		Last Modified: Tue, 24 Nov 2020 03:59:25 GMT  
		Size: 173.6 MB (173562826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b31bcb951bf4e603f2837ada0440f38d229813d9b67118437fca0f5bdd6b58`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f975e52e612075d5916bf563ca11d8ce95982baaa86c8c3e2da13b3fd7e71a`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 10.1 KB (10060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f918938a31f3e45119487cfa30fb1c1402402d8c39c644de919eec00fe597464`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 10.5 MB (10493506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:eed3db11abf068b2f5d23e7cf2c9ef6ca7a1dbb363bf1089d783b095e5d6aaca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280427439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c296a0de601cc1db9da69c6c62c6005dee80ba25360b5a9f2ab076882eb0653`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:58 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:00 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:01 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:01 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:38 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:21 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:21 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:22 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:22 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a94bca6b577989725aa37928cb1e2f8bcb96034452849a0cbb9ffb5009159a`  
		Last Modified: Tue, 24 Nov 2020 01:58:59 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c07fad3f099968bab95bf0189d7f6a3f481c13c5446de9e8f39b839b2da00`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd4714ad37fa09b0664970a83b122b03b4ebf09622a8dde6d0595ffb231b84c`  
		Last Modified: Tue, 24 Nov 2020 01:59:06 GMT  
		Size: 173.6 MB (173562256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac2cdacffdfc4bcd2b78cedaecc6e113a706ee6d44c4111609593f619a50943`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a45c2f182f51e4078348c6ba04cc7c0ec04b7de450c22c8e22bfe1abb3bc12`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 10.0 KB (10045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c01009e4beaff98f2c631248b7783aad02e8a746adf15251bce584e7e0da3c`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 10.6 MB (10584852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-slim`

```console
$ docker pull open-liberty@sha256:76d1836b9e02a305b9aec241f04ff04988e94f36e9c106926adbaff107474cb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim` - linux; amd64

```console
$ docker pull open-liberty@sha256:5c4ea2b23ff291dcedc3d2e0dbe1981ddbb10d6b448e76c64dced3e268343d97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112314228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06774cf8fdcb304d6c9d722a5a2e484c881893e3aaf1e1c0a0001ae49d9b5ae3`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:51:54 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:54 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:51:54 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:51:54 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:51:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:00 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:52:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:52:11 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:52:11 GMT
USER 1001
# Tue, 24 Nov 2020 01:52:11 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:52:11 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:52:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6b2a07158dbd6daed8528939bab7c0df681b01807294bb012efe4916610631`  
		Last Modified: Tue, 24 Nov 2020 01:57:29 GMT  
		Size: 8.1 KB (8086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485056dec16f9cfe1e0e1d351277068d7d797c3bb09119c34415cde54012288`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782d503069a74c0a09df08b77e8556b46a1549a5dc87a2edc45698519c0b169b`  
		Last Modified: Tue, 24 Nov 2020 01:57:28 GMT  
		Size: 11.6 MB (11638867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b1bf2c650fafa9492af144848a93b789affb748c8b4673543a558ffd6f04`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa51b10b6581890540bed0330311abdc2b6200912c01ef40eb21c4f75ed945d`  
		Last Modified: Tue, 24 Nov 2020 01:57:28 GMT  
		Size: 9.1 KB (9121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e1886c605697fc539432fa97700b746897bdf993d27b5ce1be27d058e631ed`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 2.5 MB (2545356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:7d5949d13ebaaee916360c4987c8c66aea5a3edf5594ac09b89d5e9171491eee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117519089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a1463eb6e194da7f2b5e231f3e9eea0b8dab7b9ebc1509b1aecd1bc420806ba`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:37:54 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 03:38:01 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:38:11 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 03:38:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:38:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:38:32 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:38:39 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:38:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:38:49 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:38:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:39:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:39:37 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:39:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:40:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:40:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:40:58 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:41:14 GMT
USER 1001
# Tue, 24 Nov 2020 03:41:20 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:41:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:41:36 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b05a8d52fa33a6297d98609b8bfcb9026069c0cbdf3da1e15b294e79c8c40f8`  
		Last Modified: Tue, 24 Nov 2020 03:58:43 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64a62e0e109ac620fab4225e3a42fdc95bc5a017d6d1700ed7882e1cee58175`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe321bd61f47be8f42586d917719b52b3be978e7b1de7ac2c39e3cead162061`  
		Last Modified: Tue, 24 Nov 2020 03:58:41 GMT  
		Size: 11.6 MB (11639707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92869bf9ec8109c338682c37e75815a3948b0162780716b990a27eb508fd4574`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed57a01c58b709a379aeed1c95a40b654f3fa1cfb54228e7e04306a9da1708f`  
		Last Modified: Tue, 24 Nov 2020 03:58:41 GMT  
		Size: 9.2 KB (9238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94b7888ef6e8630f2c0a0f0d74b953cd009c74363b0ae78059f70320259d4e8`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 2.2 MB (2232842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim` - linux; s390x

```console
$ docker pull open-liberty@sha256:3015649ac9dd909f0c06666e2404dda8ae1a3ee0e1191d3df3026732c536ff9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110150274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b050bf871675b24d7d74689a70859e96e79c3c14d5a801ecfa2ba1642d6be6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:50:30 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:50:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:50:32 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:50:32 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:50:33 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:33 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:50:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:50:34 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:50:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:50:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:50:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:50:50 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:51:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:51:01 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:51:01 GMT
USER 1001
# Tue, 24 Nov 2020 01:51:02 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:51:03 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:51:03 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e469be9ecaf59fb92177f742f7178d9a6e001e98998da741eaa7b5acc19c1c1`  
		Last Modified: Tue, 24 Nov 2020 01:58:39 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97086e240c2691f36da8d671679a262c70a61140dfeb0d711c3aee13f05e5baa`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574c871d7727cc1f9ee84fbc31d4414267faa9225d1c3cd11dcfb8d02ce0f50`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 11.6 MB (11639183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280f7d56cfed57c2191fb05d607695894162fc031ef1097ba2f2ee3a4fb5bf5d`  
		Last Modified: Tue, 24 Nov 2020 01:58:33 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60151db569e69bbc6672587ce2c590f5fb465f09a64433b09328d574783ae5e`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 9.2 KB (9220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e599c0bcd50b9ff8283f35bc47725bdc7019228d78ea6cff4b42c08974c0af5`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 2.2 MB (2232341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-slim-java11-openj9`

```console
$ docker pull open-liberty@sha256:58a82eea77fe13d30c64c58f81a00e67c88f0cbce5e64ec97dfaa761ff6be40b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:e3edd79ca3d3091e5fedd25efd89090e91557c860a606e51c9df65cc1936901b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105977814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3179c600ca25676c3079a1a73c36205a3dcc08ec288678323d495e2057c399c9`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:25:27 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:27:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:27:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:27:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:28:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:28:53 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:52:18 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:19 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:19 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:19 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:20 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:20 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:25 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:52:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:52:37 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:52:37 GMT
USER 1001
# Tue, 24 Nov 2020 01:52:37 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:52:38 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:52:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c6ae47f01d1ca61746122b9b904e8cf3d3f16e048774c5c301b535c035c87`  
		Last Modified: Wed, 28 Oct 2020 17:40:51 GMT  
		Size: 42.8 MB (42770675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bffedeca141cd6b2ed75ae8a7aea20289574815afef5089ea410c4305532a8`  
		Last Modified: Wed, 28 Oct 2020 17:40:44 GMT  
		Size: 4.4 MB (4431006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327158e7560add0f2861641f41f1c25dde9b73532cd1dfaa2ea445d7e0d8bb0d`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 8.1 KB (8089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed75dbe28c12eee9dcbec6b8c2ce34686c0a6a4a93998fe00e24d6805b5556`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242b69349c5e71e5f11a28678dbf66dba62690036cbcb2694402a2ffdd858f7f`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 11.6 MB (11638877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068137fcf68e0c921002fde603e80b9cd01d54474fbc02ad78485dcdf67c3061`  
		Last Modified: Tue, 24 Nov 2020 01:57:33 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea350bbbdb66a8b45bcaa35046d6fb107ba3f06b71d6bdefde47b9f4748f7325`  
		Last Modified: Tue, 24 Nov 2020 01:57:33 GMT  
		Size: 9.1 KB (9121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d58b0429d26cfd4bbf27ec76be282e6459bad41460414420e0c26a2e3cd632`  
		Last Modified: Tue, 24 Nov 2020 01:57:34 GMT  
		Size: 2.5 MB (2527841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:57830adb4c5f68fcf3e1912e17d9711629df86ff54c80082cea1e9b4a66431cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111674774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c72514207a11557265cd41a6bb813cd792a347e491d090f96379de5c6847f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:29:32 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:32:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:32:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:32:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:34:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:34:21 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:41:52 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:41:59 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 03:42:08 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:42:13 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 03:42:17 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:42:22 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:42:24 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:42:28 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:42:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:42:36 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:42:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:43:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:43:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:43:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:43:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:43:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:43:57 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:44:00 GMT
USER 1001
# Tue, 24 Nov 2020 03:44:03 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:44:07 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:44:10 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9518fb573dc23ad650fc0ea068af5f93f07e910761dbb8b83156f14d391027`  
		Last Modified: Wed, 28 Oct 2020 17:53:00 GMT  
		Size: 43.7 MB (43650458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7e2048088ed2d44960340a046c30cd88499c7356ea5d5da70160cb9286e6de`  
		Last Modified: Wed, 28 Oct 2020 17:52:52 GMT  
		Size: 3.5 MB (3464582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c561600f7fad28df90c2bd991668dc50f67fcaf6b516d5891f44fc5a3f2f7f`  
		Last Modified: Tue, 24 Nov 2020 03:59:00 GMT  
		Size: 8.1 KB (8116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cde82ec9eb0393ea1050e8b546f491cb0d1dec603ead8e6f09511d41b8d7d3`  
		Last Modified: Tue, 24 Nov 2020 03:58:57 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99fbfdb4883bbe55f3e5a1d4ea7ed9eec6aa66abdc17e3a96d1c9908fb7f162`  
		Last Modified: Tue, 24 Nov 2020 03:58:59 GMT  
		Size: 11.6 MB (11639707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de2b5e3f2ec46add6ccb0a98645b0594c2a9eb16469ec329c0c13c2974f9aa9`  
		Last Modified: Tue, 24 Nov 2020 03:58:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d25374215059055ce3498686857628d27bc027d52117f0b4d6eb302eddbbbf`  
		Last Modified: Tue, 24 Nov 2020 03:58:58 GMT  
		Size: 9.2 KB (9240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7929ea9a33fe8690215c31091e4fa73586b715ea9959f4646e57e74dc34ca4bd`  
		Last Modified: Tue, 24 Nov 2020 03:58:57 GMT  
		Size: 2.4 MB (2416607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:f1c1511c79a8b8ce970dfd958b4ecb3b699fb1ab88bfc99a9d6ddd72eabcc77d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103254175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e23871a3ccc0069dfd22542511020041c954d4408f61385483e0f78f95041631`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 17:47:34 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 28 Oct 2020 17:49:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b73f406dba1560dc194ac891452a1aacc2ba3b3e5e7b55e91a64559f8c2d9539';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_aarch64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='256a01e045867dcbbc541a6dd95ed315599f737b278319c4b936ce5a8a464424';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='91b74f434a3d7000dac788693f0b1e5288bd99c9bc6ef345ba6e165957defcf3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='54c845c167c197ba789eb6c3508faa5b1c95c9abe2ac26878123b6eecc87a111';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_linux_openj9_11.0.9_11_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 17:49:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 28 Oct 2020 17:51:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 28 Oct 2020 17:51:11 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:10 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:11 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:51:11 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:51:12 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:51:13 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:51:14 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:14 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:51:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:51:16 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:51:16 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:51:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:51:28 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:51:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:51:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:51:45 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:51:46 GMT
USER 1001
# Tue, 24 Nov 2020 01:51:46 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:51:47 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:51:48 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326a811af266d8284989b860fcf1e92ea12f9c383c5a2b79a622b2096ba7a7`  
		Last Modified: Wed, 28 Oct 2020 18:03:12 GMT  
		Size: 42.0 MB (42029813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d45bc780f2843a5e6d7b59b2552d62db894ec6a13ee501d17d38dfc0046a1`  
		Last Modified: Wed, 28 Oct 2020 18:03:07 GMT  
		Size: 4.1 MB (4063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98757556e5c82b0a19a8d02431b0bee29a761581c8b760de69684dd4e6ae2ea1`  
		Last Modified: Tue, 24 Nov 2020 01:58:50 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631b6f1b8592750099c773d9ef712641736935d18f41646adee537a399215b1`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8ece28373489c383503dfd5e3056d916307ce3dab6d54ae7d039951a9166f8`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 11.6 MB (11639182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78474d7ee6066218f0f4c52b426b3313862a8be50cdcc4762ddec04da89d6a8e`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e55ac2048927370e1d816cac2fef73d8eec21b0996ae36f601970747d483b7`  
		Last Modified: Tue, 24 Nov 2020 01:58:48 GMT  
		Size: 9.2 KB (9215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c3a06e7660289dbcf9b07685ca8271320197e996337eac0441fbbe9e84b197`  
		Last Modified: Tue, 24 Nov 2020 01:58:47 GMT  
		Size: 2.5 MB (2504491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:76d1836b9e02a305b9aec241f04ff04988e94f36e9c106926adbaff107474cb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:5c4ea2b23ff291dcedc3d2e0dbe1981ddbb10d6b448e76c64dced3e268343d97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112314228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06774cf8fdcb304d6c9d722a5a2e484c881893e3aaf1e1c0a0001ae49d9b5ae3`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:51:54 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:51:54 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:51:54 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:51:54 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:51:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:00 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:52:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:52:11 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:52:11 GMT
USER 1001
# Tue, 24 Nov 2020 01:52:11 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:52:11 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:52:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6b2a07158dbd6daed8528939bab7c0df681b01807294bb012efe4916610631`  
		Last Modified: Tue, 24 Nov 2020 01:57:29 GMT  
		Size: 8.1 KB (8086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485056dec16f9cfe1e0e1d351277068d7d797c3bb09119c34415cde54012288`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782d503069a74c0a09df08b77e8556b46a1549a5dc87a2edc45698519c0b169b`  
		Last Modified: Tue, 24 Nov 2020 01:57:28 GMT  
		Size: 11.6 MB (11638867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2b1bf2c650fafa9492af144848a93b789affb748c8b4673543a558ffd6f04`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa51b10b6581890540bed0330311abdc2b6200912c01ef40eb21c4f75ed945d`  
		Last Modified: Tue, 24 Nov 2020 01:57:28 GMT  
		Size: 9.1 KB (9121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e1886c605697fc539432fa97700b746897bdf993d27b5ce1be27d058e631ed`  
		Last Modified: Tue, 24 Nov 2020 01:57:27 GMT  
		Size: 2.5 MB (2545356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:7d5949d13ebaaee916360c4987c8c66aea5a3edf5594ac09b89d5e9171491eee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117519089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a1463eb6e194da7f2b5e231f3e9eea0b8dab7b9ebc1509b1aecd1bc420806ba`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:37:54 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 03:38:01 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:38:11 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 03:38:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:38:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:38:32 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:38:39 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:38:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:38:49 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:38:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:39:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:39:37 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:39:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:40:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:40:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:40:58 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:41:14 GMT
USER 1001
# Tue, 24 Nov 2020 03:41:20 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:41:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:41:36 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b05a8d52fa33a6297d98609b8bfcb9026069c0cbdf3da1e15b294e79c8c40f8`  
		Last Modified: Tue, 24 Nov 2020 03:58:43 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64a62e0e109ac620fab4225e3a42fdc95bc5a017d6d1700ed7882e1cee58175`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe321bd61f47be8f42586d917719b52b3be978e7b1de7ac2c39e3cead162061`  
		Last Modified: Tue, 24 Nov 2020 03:58:41 GMT  
		Size: 11.6 MB (11639707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92869bf9ec8109c338682c37e75815a3948b0162780716b990a27eb508fd4574`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed57a01c58b709a379aeed1c95a40b654f3fa1cfb54228e7e04306a9da1708f`  
		Last Modified: Tue, 24 Nov 2020 03:58:41 GMT  
		Size: 9.2 KB (9238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94b7888ef6e8630f2c0a0f0d74b953cd009c74363b0ae78059f70320259d4e8`  
		Last Modified: Tue, 24 Nov 2020 03:58:40 GMT  
		Size: 2.2 MB (2232842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:3015649ac9dd909f0c06666e2404dda8ae1a3ee0e1191d3df3026732c536ff9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110150274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b050bf871675b24d7d74689a70859e96e79c3c14d5a801ecfa2ba1642d6be6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c
# Tue, 24 Nov 2020 01:50:30 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:50:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip
# Tue, 24 Nov 2020 01:50:32 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:50:32 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:50:33 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:33 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:50:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:50:34 GMT
COPY dir:3229e2023f903de3453ddfbc274d32ed7322e4e9a76967a0e490dfb5f1c0fc51 in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:50:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:50:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:50:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:50:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:50:50 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:51:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/20.0.0.12/openliberty-kernel-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=bff7792697a02fe7764f2e489b4217f7a85c4b4c LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:51:01 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:51:01 GMT
USER 1001
# Tue, 24 Nov 2020 01:51:02 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:51:03 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:51:03 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e469be9ecaf59fb92177f742f7178d9a6e001e98998da741eaa7b5acc19c1c1`  
		Last Modified: Tue, 24 Nov 2020 01:58:39 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97086e240c2691f36da8d671679a262c70a61140dfeb0d711c3aee13f05e5baa`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574c871d7727cc1f9ee84fbc31d4414267faa9225d1c3cd11dcfb8d02ce0f50`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 11.6 MB (11639183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280f7d56cfed57c2191fb05d607695894162fc031ef1097ba2f2ee3a4fb5bf5d`  
		Last Modified: Tue, 24 Nov 2020 01:58:33 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60151db569e69bbc6672587ce2c590f5fb465f09a64433b09328d574783ae5e`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 9.2 KB (9220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e599c0bcd50b9ff8283f35bc47725bdc7019228d78ea6cff4b42c08974c0af5`  
		Last Modified: Tue, 24 Nov 2020 01:58:34 GMT  
		Size: 2.2 MB (2232341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:ff9b703e6b6d99f15e4056508a4bcf4228547fbcf6f89c98fd6f03bc3584b449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:d8ddf628bcd60d9d7b04037f65ae5f8cfbe4febe36d808be4d48c965dad7b3e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285245204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01dbd22d389e3f49f0bc10ff3d55c22ad57b5149814b2a05c174e3f25e4d359`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:20:44 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:22:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:22:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:24:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:24:01 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:51:53 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:52:43 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:44 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:44 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:56 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:34 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:34 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:35 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03adaffd7e576f90e30e1dede0962fbbb0b58baede693e6375c2c137e506ef92`  
		Last Modified: Wed, 28 Oct 2020 17:37:00 GMT  
		Size: 16.0 MB (16031340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168877d9653146108785fc0fae8413373c3bf38570b5e2889cb26c20c7471a79`  
		Last Modified: Thu, 19 Nov 2020 19:26:57 GMT  
		Size: 49.2 MB (49176356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63a68a33cbb86db9b0119dd1fba76f1b52451bde1540f521c6cf9e598c3887`  
		Last Modified: Thu, 19 Nov 2020 19:26:51 GMT  
		Size: 4.3 MB (4344237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b301e8e4912399d4efe9baca3d0fbbd6455c25dd47980b4ac4b8fa5cab6441a`  
		Last Modified: Tue, 24 Nov 2020 01:57:40 GMT  
		Size: 8.5 KB (8524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e04408fc6d03bf8ca6dfdebe18d700cae9fc0810e6a7cf6dff9e61d54da906`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3222a371e7cd907495e787f86a28e3afddf26ca48f45553194584f516c4f3df8`  
		Last Modified: Tue, 24 Nov 2020 01:57:50 GMT  
		Size: 173.6 MB (173562178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b79609c22cad5e21937da2fe522e3f795ed5f59c5d6fdf3cbc316ec757ff2`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a601e73fae6400ed40b14573f9e54b61d38ede651d8bf264d5de94d995c7a`  
		Last Modified: Tue, 24 Nov 2020 01:57:39 GMT  
		Size: 9.9 KB (9898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362944bb1a2ca37fb1b1dd7ffad50932be48182ee0a67b97ffd3737935ae9cd`  
		Last Modified: Tue, 24 Nov 2020 01:57:41 GMT  
		Size: 13.6 MB (13551482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:e76c103cef8a2a7038801bb40bb9b1b1d64a65b63e4016daa3351b164aa3961b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287704444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2e7bf3831e52ec23bc69904f45ef578bf14c94829832737c97510c22f78b84`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:17:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:19:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:38:23 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:43:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:44:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:46:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:48:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 03:37:51 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 03:44:30 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 03:44:33 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 03:44:35 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 03:44:38 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 03:44:42 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 03:44:46 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:44:47 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 03:44:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 03:44:50 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 03:44:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 03:45:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 03:45:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 03:46:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 03:46:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 03:47:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 03:47:23 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 03:47:28 GMT
USER 1001
# Tue, 24 Nov 2020 03:47:31 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 03:47:33 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 03:47:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82384b001eeabdc2ca426e902a10696a33f7e7723f24eca9f4848ebbe13a5e`  
		Last Modified: Wed, 28 Oct 2020 17:47:13 GMT  
		Size: 17.2 MB (17208276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f79c447f20a611d40b2f64ea6c3188f6d7dd5aeb4381c79836741f2f4d1ce`  
		Last Modified: Thu, 19 Nov 2020 20:10:00 GMT  
		Size: 49.6 MB (49603251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b5efb5095e6b26f2ac3da3dfd36d03904251df7024ad41aac8a362fd494416`  
		Last Modified: Thu, 19 Nov 2020 20:09:52 GMT  
		Size: 3.5 MB (3539881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43c793230c1bc06ea952af86e196c6c84c71921201aeaa9843fbef5ba9df34`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7302a20cb17fd50c657ad3f9830d84023e24495ebe5acea8b01ff028a806b8`  
		Last Modified: Tue, 24 Nov 2020 03:59:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702716097cf974ef7c1ad855c59c86afeda102fb9d42e48ffe786a7a899afb0d`  
		Last Modified: Tue, 24 Nov 2020 03:59:25 GMT  
		Size: 173.6 MB (173562826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b31bcb951bf4e603f2837ada0440f38d229813d9b67118437fca0f5bdd6b58`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f975e52e612075d5916bf563ca11d8ce95982baaa86c8c3e2da13b3fd7e71a`  
		Last Modified: Tue, 24 Nov 2020 03:59:08 GMT  
		Size: 10.1 KB (10060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f918938a31f3e45119487cfa30fb1c1402402d8c39c644de919eec00fe597464`  
		Last Modified: Tue, 24 Nov 2020 03:59:11 GMT  
		Size: 10.5 MB (10493506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:eed3db11abf068b2f5d23e7cf2c9ef6ca7a1dbb363bf1089d783b095e5d6aaca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280427439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c296a0de601cc1db9da69c6c62c6005dee80ba25360b5a9f2ab076882eb0653`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 23 Oct 2020 19:09:19 GMT
ADD file:9b934c86e9ab1dd29cef318d8dd9cd1228b9d92124f434c50ad7d03ede1a5c76 in / 
# Fri, 23 Oct 2020 19:09:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:09:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:09:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:09:27 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 17:41:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 28 Oct 2020 17:41:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 19:43:34 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Thu, 19 Nov 2020 19:45:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44d9feb46d613b55a8b7f249bbf5c5db27102e21a2fb64c5af72d1742a27b808';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_aarch64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8003472eb7f44d401cea9d3258ee5d5e55e38707c5b9c0b292d672e801325440';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        s390x)          ESUM='3f02a8bcb9ebad4061a4bf4600b6af0670e08ad87f75adb9adf7556035943195';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_s390x_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        amd64|x86_64)          ESUM='75850de26fe76a1686f838403a34b67925c573fddc492ecee0b752d30ee2545a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_linux_openj9_8u275b01_openj9-0.23.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 19:45:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Thu, 19 Nov 2020 19:47:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 19 Nov 2020 19:47:22 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 24 Nov 2020 01:50:29 GMT
ARG LIBERTY_VERSION=20.0.0.12
# Tue, 24 Nov 2020 01:51:58 GMT
ARG LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_BUILD_LABEL=cl201220201111-0736
# Tue, 24 Nov 2020 01:51:59 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip
# Tue, 24 Nov 2020 01:52:00 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 24 Nov 2020 01:52:01 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 24 Nov 2020 01:52:01 GMT
ARG OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:02 GMT
ARG VERBOSE=false
# Tue, 24 Nov 2020 01:52:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl201220201111-0736 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.12
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:7aff51efcc7f992aebc75df1ed45eed67c8a6f2121249c7fc7b35f23cc108b3d in /opt/ol/helpers 
# Tue, 24 Nov 2020 01:52:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 24 Nov 2020 01:52:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 24 Nov 2020 01:52:38 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 24 Nov 2020 01:52:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 24 Nov 2020 01:52:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 24 Nov 2020 01:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl201220201111-0736 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.12/openliberty-runtime-20.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=18deec3a143a6a2ac46c717722a90678c524fa4e LIBERTY_VERSION=20.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 24 Nov 2020 01:53:21 GMT
ENV RANDFILE=/tmp/.rnd
# Tue, 24 Nov 2020 01:53:21 GMT
USER 1001
# Tue, 24 Nov 2020 01:53:22 GMT
EXPOSE 9080 9443
# Tue, 24 Nov 2020 01:53:22 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 24 Nov 2020 01:53:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d3e8e1a5d50716d6aabb0cef46599f9e7a722a560910d6f724737aaef0a7d6c3`  
		Last Modified: Mon, 12 Oct 2020 16:45:31 GMT  
		Size: 27.2 MB (27224393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04282efaafb3c9b53bba677fc3c06c478dc1613c1f21939bfa2c113aeef2f99c`  
		Last Modified: Fri, 23 Oct 2020 19:10:20 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6269ae100536d7559ae6ebe6606b4405ebb706c3d963926c5568b6e7fd954582`  
		Last Modified: Fri, 23 Oct 2020 19:10:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd8065d26d8f90607b2debf915de6242befbe898f8fb305dbd99dc8df92d3a`  
		Last Modified: Wed, 28 Oct 2020 17:59:30 GMT  
		Size: 15.8 MB (15772935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0b1fbe0a76f4faf6a1c8bc5e39d2af4c37d0008acc2423ef0e7890a22ad931`  
		Last Modified: Thu, 19 Nov 2020 19:51:05 GMT  
		Size: 48.8 MB (48789618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db73010105b38fe1b46be46b1363f5412190449bb56d6a5709d6c5972e76801`  
		Last Modified: Thu, 19 Nov 2020 19:50:59 GMT  
		Size: 4.5 MB (4472229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a94bca6b577989725aa37928cb1e2f8bcb96034452849a0cbb9ffb5009159a`  
		Last Modified: Tue, 24 Nov 2020 01:58:59 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c07fad3f099968bab95bf0189d7f6a3f481c13c5446de9e8f39b839b2da00`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd4714ad37fa09b0664970a83b122b03b4ebf09622a8dde6d0595ffb231b84c`  
		Last Modified: Tue, 24 Nov 2020 01:59:06 GMT  
		Size: 173.6 MB (173562256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac2cdacffdfc4bcd2b78cedaecc6e113a706ee6d44c4111609593f619a50943`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a45c2f182f51e4078348c6ba04cc7c0ec04b7de450c22c8e22bfe1abb3bc12`  
		Last Modified: Tue, 24 Nov 2020 01:58:56 GMT  
		Size: 10.0 KB (10045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c01009e4beaff98f2c631248b7783aad02e8a746adf15251bce584e7e0da3c`  
		Last Modified: Tue, 24 Nov 2020 01:58:58 GMT  
		Size: 10.6 MB (10584852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
