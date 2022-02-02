<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `open-liberty`

-	[`open-liberty:21.0.0.12-full-java11-openj9`](#open-liberty210012-full-java11-openj9)
-	[`open-liberty:21.0.0.12-full-java8-openj9`](#open-liberty210012-full-java8-openj9)
-	[`open-liberty:21.0.0.12-kernel-slim-java11-openj9`](#open-liberty210012-kernel-slim-java11-openj9)
-	[`open-liberty:21.0.0.12-kernel-slim-java8-openj9`](#open-liberty210012-kernel-slim-java8-openj9)
-	[`open-liberty:21.0.0.9-full-java11-openj9`](#open-liberty21009-full-java11-openj9)
-	[`open-liberty:21.0.0.9-full-java8-openj9`](#open-liberty21009-full-java8-openj9)
-	[`open-liberty:21.0.0.9-kernel-slim-java11-openj9`](#open-liberty21009-kernel-slim-java11-openj9)
-	[`open-liberty:21.0.0.9-kernel-slim-java8-openj9`](#open-liberty21009-kernel-slim-java8-openj9)
-	[`open-liberty:22.0.0.1-full-java11-openj9`](#open-liberty22001-full-java11-openj9)
-	[`open-liberty:22.0.0.1-full-java8-openj9`](#open-liberty22001-full-java8-openj9)
-	[`open-liberty:22.0.0.1-kernel-slim-java11-openj9`](#open-liberty22001-kernel-slim-java11-openj9)
-	[`open-liberty:22.0.0.1-kernel-slim-java8-openj9`](#open-liberty22001-kernel-slim-java8-openj9)
-	[`open-liberty:beta`](#open-libertybeta)
-	[`open-liberty:beta-java11`](#open-libertybeta-java11)
-	[`open-liberty:full`](#open-libertyfull)
-	[`open-liberty:full-java11-openj9`](#open-libertyfull-java11-openj9)
-	[`open-liberty:full-java8-openj9`](#open-libertyfull-java8-openj9)
-	[`open-liberty:kernel-slim`](#open-libertykernel-slim)
-	[`open-liberty:kernel-slim-java11-openj9`](#open-libertykernel-slim-java11-openj9)
-	[`open-liberty:kernel-slim-java8-openj9`](#open-libertykernel-slim-java8-openj9)
-	[`open-liberty:latest`](#open-libertylatest)

## `open-liberty:21.0.0.12-full-java11-openj9`

```console
$ docker pull open-liberty@sha256:0044f6b766b08cd402ec8a04d711a805c6f0398f2a0734b3c0cacd8ede4801a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.12-full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:2f6fed1f5985a2997b56dab859846dbc8c3267e810f5240ec7265f67717a361d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.5 MB (396473859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f469caac5ce508a3f7975c5af63b1d0ef945e4c6ed258f49a590a3dd1a39d73`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:18:50 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Tue, 01 Feb 2022 02:20:11 GMT
ARG LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b
# Tue, 01 Feb 2022 02:20:12 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:20:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip
# Tue, 01 Feb 2022 02:20:12 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:20:12 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:20:12 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:20:13 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:20:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Tue, 01 Feb 2022 02:20:13 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:20:13 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:20:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:20:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:20:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:20:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:21:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:21:01 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:21:02 GMT
USER 1001
# Tue, 01 Feb 2022 02:21:02 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:21:02 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:21:02 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000fcde4054e4c30053e4d487cfce4b65e505ecba62d9a6f21039632760fdd9c`  
		Last Modified: Tue, 01 Feb 2022 02:27:06 GMT  
		Size: 8.6 KB (8553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81035a01325db8ce2c75b85130bc3b1e694d813c5b7ed6ba3328d53c8ebc88ad`  
		Last Modified: Tue, 01 Feb 2022 02:27:04 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ccd5ca2d933b30e303b93f0d2f2b08f087dd07e44b64ab62d4b9320cdbd48`  
		Last Modified: Tue, 01 Feb 2022 02:27:19 GMT  
		Size: 285.7 MB (285734968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13380e482d7ee5571593e5c94063bc3f209f8d50c9f42b24b66beaa3f88d62dd`  
		Last Modified: Tue, 01 Feb 2022 02:27:04 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6042bab3b79a1d761d9eaa5af9df2b5f1b01f2a227d89d8bf2b7c11bbd2b6e57`  
		Last Modified: Tue, 01 Feb 2022 02:27:04 GMT  
		Size: 10.0 KB (10042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ecacec6fd69958460e4ded4ca032006a754d29b399640e859f4953b5b9966`  
		Last Modified: Tue, 01 Feb 2022 02:27:07 GMT  
		Size: 14.0 MB (14004912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:a7b136cb6da45d09de81729f37204ad464a9e26bc7ae95764e3a2c7acdd59612
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **400.1 MB (400098730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc3ebca0cb55fb808f0edf8bb1859881accd7514ef138d13286860b473806c9`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:09:27 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 14:18:20 GMT
ARG LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b
# Wed, 02 Feb 2022 14:18:24 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 14:18:28 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip
# Wed, 02 Feb 2022 14:18:32 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:18:36 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:18:40 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:18:45 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:18:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 14:18:51 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:18:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:21:50 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:21:58 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:22:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:22:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:23:10 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:23:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:23:18 GMT
USER 1001
# Wed, 02 Feb 2022 14:23:21 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:23:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:23:27 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b179f30f578835354f8ecbde23d2bdafcf0f1eeccf6d0b94f4baacc9311b0ba`  
		Last Modified: Wed, 02 Feb 2022 14:51:34 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a73e61269fcc26293647dcd124bdb84eaac660164f42059c74e81dbe362229`  
		Last Modified: Wed, 02 Feb 2022 14:51:31 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797dbdecd78716ee1bebf14d6b141dc5dd5d5b9dea73b901538ff21ce4e38637`  
		Last Modified: Wed, 02 Feb 2022 14:51:56 GMT  
		Size: 285.7 MB (285735564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe7cc36a2f8aacafa314bc1e0b460393f511980f0e7d428e5eb7be26fb18a40`  
		Last Modified: Wed, 02 Feb 2022 14:51:31 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877511260dad4f44c08ea7f638a268e39d8acfe3cbcde41e8cbb0d824236f53a`  
		Last Modified: Wed, 02 Feb 2022 14:51:32 GMT  
		Size: 10.1 KB (10068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed70e85ca0a77e59e2a7477b56244bff45a4b1105e443e10f70170a073dfb993`  
		Last Modified: Wed, 02 Feb 2022 14:51:34 GMT  
		Size: 12.2 MB (12177993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:82bbd2c311768ae1d2a5c55f5a92d226ba9ec0ed1fcec2b03c1de2984c3c6500
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.3 MB (393336461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6904182aa880a3d75e6a36c63d493e687152d842c0e017e0dfcb155badcfe2`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 05:00:08 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 05:01:55 GMT
ARG LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b
# Wed, 02 Feb 2022 05:01:55 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:01:55 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip
# Wed, 02 Feb 2022 05:01:56 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:01:56 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:01:56 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:01:56 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:01:56 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 05:01:56 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:01:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:02:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:02:17 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:02:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:02:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:02:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:02:40 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:02:40 GMT
USER 1001
# Wed, 02 Feb 2022 05:02:41 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:02:41 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:02:41 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b89701495dc513bb10395bef64b6f28b9fe3ed9d47db488b765f1968863ef40`  
		Last Modified: Wed, 02 Feb 2022 05:08:14 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eff6df9e62533bf84711b33610b4fd165768f8489192bc0490c1e4667f788b1`  
		Last Modified: Wed, 02 Feb 2022 05:08:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86ffa1193530d2f3dc60dc53b1d2e07e16e882c66263fe27990c581923f02b`  
		Last Modified: Wed, 02 Feb 2022 05:08:25 GMT  
		Size: 285.7 MB (285735141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9970f4b8f5cfd796114d93b88f018d83190bd66b4a7d66b3715c2e71d1aaed6`  
		Last Modified: Wed, 02 Feb 2022 05:08:13 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015e2cf167a00d839760f344d156e44e56149f322af07edff2af0e356d066811`  
		Last Modified: Wed, 02 Feb 2022 05:08:13 GMT  
		Size: 10.0 KB (10037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04852a328196677d94343fda7ef41814b294823c56852a6246712f7491714d54`  
		Last Modified: Wed, 02 Feb 2022 05:08:14 GMT  
		Size: 13.8 MB (13750648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.12-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:101b794f90823e79c3cb2477f3f98335975eb3b73f3d120f35870ec90fad9af2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.12-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:c5f7b00a1a34310342493b271fee920fad9d46a534344e9ea229e37956308294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.0 MB (397969007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aeda0331ea538df779d7a1d9fa000da8ae843dd0919be4f990cd2a79c709e32`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:18:31 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Tue, 01 Feb 2022 02:19:14 GMT
ARG LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b
# Tue, 01 Feb 2022 02:19:14 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:19:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip
# Tue, 01 Feb 2022 02:19:14 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:19:15 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:19:15 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:19:15 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:19:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Tue, 01 Feb 2022 02:19:15 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:19:16 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:19:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:19:29 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:19:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:19:31 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:20:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:20:02 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:20:02 GMT
USER 1001
# Tue, 01 Feb 2022 02:20:03 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:20:03 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:20:03 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee59ea79355429bc63d487f718586499dca146adaa419ee5ef8bacf76fe143c5`  
		Last Modified: Tue, 01 Feb 2022 02:26:45 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b71e2fbe4ba60bd9bb22aade493170f6ca31fe9233c4f3ebb8b2e02f7d2a9`  
		Last Modified: Tue, 01 Feb 2022 02:26:42 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e65042953ab4b9fb105fcecac0d0b7d3b64c922fbaf725e7d20c3735f69fa8`  
		Last Modified: Tue, 01 Feb 2022 02:26:56 GMT  
		Size: 285.7 MB (285734964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6655f0d414e634be28b8ef936db982ac786954c109f7113495b2be2da2f315e1`  
		Last Modified: Tue, 01 Feb 2022 02:26:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73767daec90df58099cb28e58dfc32e2cfe07bdbb3812230ec83854a73ba2067`  
		Last Modified: Tue, 01 Feb 2022 02:26:42 GMT  
		Size: 10.0 KB (10043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9ae3255e43a4f6a3fb970b8face78b43821ff89c3ad8d9935f561bbb5b8331`  
		Last Modified: Tue, 01 Feb 2022 02:26:45 GMT  
		Size: 13.4 MB (13390214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:a7c40ce5538a401d10142947f98a0d838a977fcff207c71233f0cace6feaedb5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.1 MB (402142096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcf122e44e4afb793b0c104e2f20859c603c8fa78abb060e9d50506991cec562`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:05:32 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 14:13:10 GMT
ARG LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b
# Wed, 02 Feb 2022 14:13:14 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 14:13:19 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip
# Wed, 02 Feb 2022 14:13:26 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:13:30 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:13:34 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:13:37 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:13:39 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 14:13:41 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:13:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:16:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:16:38 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:16:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:17:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:17:49 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:17:52 GMT
USER 1001
# Wed, 02 Feb 2022 14:17:56 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:17:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:18:02 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175c3e800d1e584e11540428a07245e8b810118e8113d477f6287c7b53fe583`  
		Last Modified: Wed, 02 Feb 2022 14:51:01 GMT  
		Size: 8.6 KB (8553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcd46330146ba1105ce00bc6d94591ef532e33796fd22b20157ac153d76138`  
		Last Modified: Wed, 02 Feb 2022 14:50:57 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c1c6b81757043727bb28071b6f4123cf6eaa106da0f86334a2d22083d18f4`  
		Last Modified: Wed, 02 Feb 2022 14:51:22 GMT  
		Size: 285.7 MB (285735576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc597f547d9e1ee1424024d0be949540b6bef6d99051f45e18bb0cdcbd5afdd`  
		Last Modified: Wed, 02 Feb 2022 14:50:57 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fceea3f2c79795b6ea186e9d9fa0940571dfb809812651a5de8a24d162a812ca`  
		Last Modified: Wed, 02 Feb 2022 14:50:58 GMT  
		Size: 10.1 KB (10073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a17ecd38c7e1e5e46d3b2ef28ac431a700209b418cc2cd6fb9fb5c6763f4ff`  
		Last Modified: Wed, 02 Feb 2022 14:51:00 GMT  
		Size: 12.0 MB (11965202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:4b4ab9061193ee4690fe02cd26fde9705c258e9637020e0744de1162d44f69db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.9 MB (392910504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e12ec74a4ab9938608957ffb4518c1f5683ca4cde7ae7a842ce8000935ba130`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:59:09 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 05:00:32 GMT
ARG LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b
# Wed, 02 Feb 2022 05:00:33 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:00:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip
# Wed, 02 Feb 2022 05:00:33 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:00:33 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:00:33 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:00:33 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:00:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 05:00:34 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:00:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:01:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:01:26 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:01:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:01:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:01:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.12/openliberty-runtime-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=85635806bc4acc7192ea4d542d67462182e8fa3b LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:01:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:01:46 GMT
USER 1001
# Wed, 02 Feb 2022 05:01:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:01:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:01:47 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7061a52024a3ce5c3202a95a37967b7dce3101e6d2a8e6355fe912b485e9b7`  
		Last Modified: Wed, 02 Feb 2022 05:07:56 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b07e2d45cd810d1b1809333802152052d80b30fd2b1d53c4464c37e63db62c`  
		Last Modified: Wed, 02 Feb 2022 05:07:55 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee7b704235473fc5271eb604e987e1b996767d601faa5ed4ede892f2d70024d`  
		Last Modified: Wed, 02 Feb 2022 05:08:07 GMT  
		Size: 285.7 MB (285735152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5260493105cf17f1ae9cb93bd7858892e2f0d45c20379de2ea9aab3b9f93cf78`  
		Last Modified: Wed, 02 Feb 2022 05:07:55 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da87a757c9a2c54901a2cadae5a5b9b8e0e25dbb3db9ed8bcb1e4dcbf516a389`  
		Last Modified: Wed, 02 Feb 2022 05:07:55 GMT  
		Size: 10.1 KB (10052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bbe5d8aba6d415117c04692506f6f7be0de47fd1321c06f98b00a561a4bfaa`  
		Last Modified: Wed, 02 Feb 2022 05:07:56 GMT  
		Size: 10.8 MB (10797245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.12-kernel-slim-java11-openj9`

```console
$ docker pull open-liberty@sha256:200ed4cfbfd8c4a55dca746dc113d119febc3bf75391362903a4ae46ccf8e75c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.12-kernel-slim-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:81458983ff47cc2b3a90578aa49c4394df15c62586e0fc879425a10a9c0269b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111063744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9f616019076238029bf21e77df38bfd2c38f0c21772c98bb27c85c6d4ad7fd`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:18:50 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Tue, 01 Feb 2022 02:18:51 GMT
ARG LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e
# Tue, 01 Feb 2022 02:18:51 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:18:51 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip
# Tue, 01 Feb 2022 02:18:51 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:18:51 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:18:52 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:18:52 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:18:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Tue, 01 Feb 2022 02:18:52 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:18:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:18:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:18:58 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:18:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:19:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:19:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:19:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:19:08 GMT
USER 1001
# Tue, 01 Feb 2022 02:19:08 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:19:09 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:19:09 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c29469ffa1d9560e60a8c535c7103ffab1e5e8dccfbb572b5e522bc642ea716`  
		Last Modified: Tue, 01 Feb 2022 02:26:35 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b609e8b9fc9691c31de9eb32315186c2ebf4ce8732122923030c6c93e4cf793f`  
		Last Modified: Tue, 01 Feb 2022 02:26:33 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3cb235997efe9f0db850719b2d7e75dd937be1c792eaac8adef5af73081ae2`  
		Last Modified: Tue, 01 Feb 2022 02:26:34 GMT  
		Size: 11.8 MB (11827270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521ec9c3345802bcc0e51fbe1eff582b41cf4828c9ecea54b2b14607518f91d9`  
		Last Modified: Tue, 01 Feb 2022 02:26:33 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cd39b5d7d012bc39991b5ca04ffd682258fe9aaf2c7f0b74a40b82027f6b92`  
		Last Modified: Tue, 01 Feb 2022 02:26:33 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8d783c6e17daa6d40243264eaef0cce0095565c4078e7ecfb7093f37b6c136`  
		Last Modified: Tue, 01 Feb 2022 02:26:34 GMT  
		Size: 2.5 MB (2504090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-kernel-slim-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:05beebab2c274cb5c4f4674d64ec06a8bc05b3ee29bf81eed3c71c89f900748e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116437739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57944e73efbbe5340ce02e15e213c295f1fa1478692a4ddc39541c9386e6926`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:09:27 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 14:09:29 GMT
ARG LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e
# Wed, 02 Feb 2022 14:09:31 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 14:09:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip
# Wed, 02 Feb 2022 14:09:35 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:09:37 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:09:40 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:09:42 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:09:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 14:09:45 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:09:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:12:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:12:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:12:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:12:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:12:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:12:44 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:12:47 GMT
USER 1001
# Wed, 02 Feb 2022 14:12:49 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:12:50 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:12:53 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e21ed424cbe2ca3c098e9d27008c2bfcb681adc97f68b165e2c6701a0a2c74b`  
		Last Modified: Wed, 02 Feb 2022 14:50:49 GMT  
		Size: 8.1 KB (8115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4308e223aa323a5a2dc099702e5d4127064a8bebf2c26185a8fc42133cfbc083`  
		Last Modified: Wed, 02 Feb 2022 14:50:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb8164579e825fae9ea25a8beb1984587f23b4f454211231c4f17faea21f12f`  
		Last Modified: Wed, 02 Feb 2022 14:50:47 GMT  
		Size: 11.8 MB (11827908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd8e1156764887e8a6012b3a5395807ddce7b8f80c9de4d86d34dad6cc11ffc`  
		Last Modified: Wed, 02 Feb 2022 14:50:46 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b40e1737cbdf71b33c6017319b96c62949a3e767d7d56da4ec52051d6f10480`  
		Last Modified: Wed, 02 Feb 2022 14:50:46 GMT  
		Size: 9.2 KB (9234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd25bfed47aac5bc74ef312c063edf729770ba2da5b7a24ff8f530f9458746b1`  
		Last Modified: Wed, 02 Feb 2022 14:50:47 GMT  
		Size: 2.4 MB (2426242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-kernel-slim-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:317bc16dfcf1feefec307998270f8e5ef10878ce2d6e723954cba7e8574fdd26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108174239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93eefbe8af5f1e33bcd04cc4d6e59428155fea5069e6bc89b560e62faafb35c6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 05:00:08 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 05:00:08 GMT
ARG LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e
# Wed, 02 Feb 2022 05:00:08 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:00:08 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip
# Wed, 02 Feb 2022 05:00:09 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:00:09 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:00:09 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:00:09 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:00:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 05:00:09 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:00:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:00:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:00:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:00:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:00:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:00:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:00:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:00:25 GMT
USER 1001
# Wed, 02 Feb 2022 05:00:25 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:00:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:00:26 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712846925686adfa3dfcb3dbe7b3bff6f6a3c4bfbaaa562b5a001c518ca1c571`  
		Last Modified: Wed, 02 Feb 2022 05:07:51 GMT  
		Size: 8.1 KB (8112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac08a45ba2ef8311e91e39bdfed023e6a7ce6e3cc43d79a2e771901ff71b0d9`  
		Last Modified: Wed, 02 Feb 2022 05:07:50 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a519bce955506a42094752ec0c5e3ed260f99b08e98913f8cb691330606cbea4`  
		Last Modified: Wed, 02 Feb 2022 05:07:50 GMT  
		Size: 11.8 MB (11827479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf06914e9cf0dc0f4971c1efd5f4a9a1679a818ed35ffa9fe4f3c8365de6ae5`  
		Last Modified: Wed, 02 Feb 2022 05:07:50 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08dca6e6ad4726babed5fbc16e9de53384925f13322f140625013259e348fdd`  
		Last Modified: Wed, 02 Feb 2022 05:07:50 GMT  
		Size: 9.2 KB (9210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc27ac91fc04ad04c11cdb336bfa85eb009e7f28ef246ab23020fe4d0134c1`  
		Last Modified: Wed, 02 Feb 2022 05:07:50 GMT  
		Size: 2.5 MB (2497669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.12-kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:62631f069ec9db7c876eed14cab5b9f43d4e2c9f719dd5fb6b4554ebc0cef8dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.12-kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:db2842c75e164e71d37cc6ff577da2bf35f54f124f9568b5a2b9f3faa0a4374e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113129502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8775bb5a55b0fd6ef1aa749118313e54e0b5bb56f1199946ce43361f029409a7`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:18:31 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Tue, 01 Feb 2022 02:18:31 GMT
ARG LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e
# Tue, 01 Feb 2022 02:18:31 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:18:32 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip
# Tue, 01 Feb 2022 02:18:32 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:18:32 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:18:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:18:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:18:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Tue, 01 Feb 2022 02:18:33 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:18:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:18:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:18:39 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:18:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:18:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:18:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:18:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:18:47 GMT
USER 1001
# Tue, 01 Feb 2022 02:18:47 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:18:48 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:18:48 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0960d2e675b7c86aefcac50b2478a3a6a33871d0cbb18d0b571798aed666be`  
		Last Modified: Tue, 01 Feb 2022 02:26:26 GMT  
		Size: 8.1 KB (8110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f579537d8496630688cf02a7fc0cc94d262d9d3b6255736b5f671520fc5ac6`  
		Last Modified: Tue, 01 Feb 2022 02:26:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57351d94e09295005150c5e9d1c019c23afcbe827ae6822f9b64818c5a637143`  
		Last Modified: Tue, 01 Feb 2022 02:26:25 GMT  
		Size: 11.8 MB (11827257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93828ca75a715c20a2378a8f173b9cbbc57b69bece3a8fe69ea4b10ee8e76bf`  
		Last Modified: Tue, 01 Feb 2022 02:26:24 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fc9e6cd99689eae1aefb36e364e6823632ae8c57a36593b7e1fc180baad029`  
		Last Modified: Tue, 01 Feb 2022 02:26:24 GMT  
		Size: 9.2 KB (9213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c135041a3f906584d41bfe4dbc818cef3558351af819833c40e6f5fbb0ba2b`  
		Last Modified: Tue, 01 Feb 2022 02:26:25 GMT  
		Size: 2.5 MB (2460010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:1d007e0121c98d8f9eec8290d5d8a165e52c4325d333820d32cbc0ed404bd687
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118679886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6af2d97cbc80faf805762eb55eccc8177d139c47cbb613fd97288c19cd2a6f9a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:05:32 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 14:05:35 GMT
ARG LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e
# Wed, 02 Feb 2022 14:05:38 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 14:05:39 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip
# Wed, 02 Feb 2022 14:05:40 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:05:42 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:05:44 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:05:46 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:05:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 14:05:49 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:05:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:08:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:08:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:08:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:08:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:08:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:08:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:08:55 GMT
USER 1001
# Wed, 02 Feb 2022 14:09:00 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:09:04 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:09:06 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd190ff5e56fbe003783103ed6fa46575678c3a595d607a5408701c2dd1e1d30`  
		Last Modified: Wed, 02 Feb 2022 14:50:37 GMT  
		Size: 8.1 KB (8115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75d85fd4a2ec552a54d30fdeb29c682750a769e8043722194ea1b1fd1e10e5b`  
		Last Modified: Wed, 02 Feb 2022 14:50:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeba107dbccd953535c6a5f03fc860b404e25b7e9918ad92acfcc88161fb816`  
		Last Modified: Wed, 02 Feb 2022 14:50:36 GMT  
		Size: 11.8 MB (11827931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e33303079e1710808438b16a4785e1799ba723f951356c79b646b387e28c05`  
		Last Modified: Wed, 02 Feb 2022 14:50:34 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775e4120d16b882c11afbdfcab48c04f097b5f7b61e4dc901d313d3ecd755da2`  
		Last Modified: Wed, 02 Feb 2022 14:50:34 GMT  
		Size: 9.2 KB (9238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbb8546b20bf1001dc92161854811bb5759943b476f4c28985bf4d69fe8bcea`  
		Last Modified: Wed, 02 Feb 2022 14:50:35 GMT  
		Size: 2.4 MB (2412230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.12-kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:2c7994faa90a559fe48714ee6bf4ddc8a049192b4fbf4090311d02f976c9efe3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110445488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085f2b0d209768d3d38cf1986b3852bb66589b64df62bb03d89e75c8fdb42279`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:59:09 GMT
ARG LIBERTY_VERSION=21.0.0.12
# Wed, 02 Feb 2022 04:59:09 GMT
ARG LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e
# Wed, 02 Feb 2022 04:59:09 GMT
ARG LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 04:59:09 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip
# Wed, 02 Feb 2022 04:59:10 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:59:10 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:59:10 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:59:10 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:59:10 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.12
# Wed, 02 Feb 2022 04:59:10 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:59:10 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:59:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:59:53 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:59:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:59:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:59:59 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl21.0.0.12920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.12/openliberty-kernel-21.0.0.12.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=101f7be5f15f14a4a3dabc74dd106be2e743245e LIBERTY_VERSION=21.0.0.12 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:59:59 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:59:59 GMT
USER 1001
# Wed, 02 Feb 2022 04:59:59 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:59:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:59:59 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cb7fe295a8a86ac08229083fa66de2bcf821a32154d981942ed05c3708a202`  
		Last Modified: Wed, 02 Feb 2022 05:07:45 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1455eac0c58acb27b4d613a935cd795bdf121808e8a4441946096de5b8a966bc`  
		Last Modified: Wed, 02 Feb 2022 05:07:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1564c86786a69eb123cf598542d039cd9fef1d753a8dd8fd50e391aa655049`  
		Last Modified: Wed, 02 Feb 2022 05:07:45 GMT  
		Size: 11.8 MB (11827499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67524141e86d2c3b03f20845fc2c4211b863e8cda83e6bd4aaad8b0381c5406f`  
		Last Modified: Wed, 02 Feb 2022 05:07:44 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f777f34d17e304c23dcdef0c69a1d51811de6c29a8bc48872efaf0cfbc609b`  
		Last Modified: Wed, 02 Feb 2022 05:07:44 GMT  
		Size: 9.2 KB (9222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416b44d0f35adaca9a9c50c579dbe6d67a8d0bd392041336685bdc8c1adb7cb5`  
		Last Modified: Wed, 02 Feb 2022 05:07:45 GMT  
		Size: 2.2 MB (2241475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.9-full-java11-openj9`

```console
$ docker pull open-liberty@sha256:ec3ad337398290d0840b9b13baa781c17f871c981cf54a9d34fe0ee93bbec6b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.9-full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:637b1e3daaaa967276a1214a7a3f45ce40384339f47aed5ab559390dd101a303
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295617504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84e4fff8861d7403880b68c1aaa4c3688debd8ed6bfcae7d7e44962b0612e49`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:21:28 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Tue, 01 Feb 2022 02:22:49 GMT
ARG LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa
# Tue, 01 Feb 2022 02:22:49 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Tue, 01 Feb 2022 02:22:50 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip
# Tue, 01 Feb 2022 02:22:50 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:22:50 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:22:50 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:22:50 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:22:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Tue, 01 Feb 2022 02:22:51 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:22:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:23:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:23:02 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:23:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:23:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:23:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:23:37 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:23:37 GMT
USER 1001
# Tue, 01 Feb 2022 02:23:37 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:23:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:23:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ef92e991e90cccf17640b081c3abceae884f856860d2737a39dfcdb61a1aad`  
		Last Modified: Tue, 01 Feb 2022 02:28:02 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28780dd89eff017a5c45e00115c47c84cdc61c9adffcb78f461f243da2895223`  
		Last Modified: Tue, 01 Feb 2022 02:28:00 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92db57210e894b14b142750ad3d39d31275588151ec50e9cdfc3009bfd824bb`  
		Last Modified: Tue, 01 Feb 2022 02:28:10 GMT  
		Size: 185.1 MB (185114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa0a2cba70113640e122d5910255f0fa3c1734371d8ed42f69a3b059a37eaac`  
		Last Modified: Tue, 01 Feb 2022 02:28:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79330d5676b3a6b5fe9cc8d0aeebc847966db416b03c29874e239755af1bf0bd`  
		Last Modified: Tue, 01 Feb 2022 02:28:00 GMT  
		Size: 10.1 KB (10057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dde40a858a009a3adf497c20f3ad25bad0f5a29ab3b89bbe51a531f61ab5c3`  
		Last Modified: Tue, 01 Feb 2022 02:28:03 GMT  
		Size: 13.8 MB (13768638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:274af0fbc6461fa6901267508b91af68640b6ae1a66a8dda5a7458795d10a26a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.5 MB (299458988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94349eaf0de535f1a04c2b14c1b7a50320522392733d8f9640be9495039a3e37`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:27:58 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 14:41:34 GMT
ARG LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa
# Wed, 02 Feb 2022 14:41:43 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 14:41:48 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip
# Wed, 02 Feb 2022 14:41:51 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:41:54 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:41:58 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:42:03 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:42:05 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 14:42:06 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:42:08 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:44:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:44:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:44:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:44:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:45:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:45:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:45:54 GMT
USER 1001
# Wed, 02 Feb 2022 14:45:58 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:46:01 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:46:05 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f02e421a4722e42b9eddc9462fffdbb8a984ad07df7e1bca7b267299c42382f`  
		Last Modified: Wed, 02 Feb 2022 14:52:58 GMT  
		Size: 8.6 KB (8554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d501de55af0832682ccf3d4390d78b15ce286d79a4919ff4444d902193be996`  
		Last Modified: Wed, 02 Feb 2022 14:52:55 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c7e13047bf45e71b7c1376a2a47e43eb8a49fce086390cdc93e5afcf26db3d`  
		Last Modified: Wed, 02 Feb 2022 14:53:11 GMT  
		Size: 185.1 MB (185115535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7cd0aed7445d94bc4f1d93eeeeb2e6c7b1aa7537cc1d2eed24bd090c05c20d`  
		Last Modified: Wed, 02 Feb 2022 14:52:55 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6d20df8524b0352977901fb8a4758fae3b25e3f80a0a03aa9951fb6e158714`  
		Last Modified: Wed, 02 Feb 2022 14:52:55 GMT  
		Size: 10.1 KB (10063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a150c6700fe1b592d3d3ef5f5894b23c0ed384c6207cbca42779530de2c67f`  
		Last Modified: Wed, 02 Feb 2022 14:52:57 GMT  
		Size: 12.2 MB (12158281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:6f91a5e720a7bc406e7d4ee84957262214dbf147a9ae08855923ed90c6646c8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292708916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5343085472f59e7c61ac5b0a5b2dd66fc94151f473d51c3b01603b8d4888a380`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 05:03:16 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 05:04:29 GMT
ARG LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa
# Wed, 02 Feb 2022 05:04:29 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 05:04:29 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip
# Wed, 02 Feb 2022 05:04:29 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:04:29 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:04:29 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:04:29 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:04:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 05:04:30 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:04:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:04:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:04:46 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:04:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:04:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:05:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:05:10 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:05:11 GMT
USER 1001
# Wed, 02 Feb 2022 05:05:11 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:05:11 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:05:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f813903f0dbe3df45346c7065076006095144925c28f9ff06ca9d68fe03b08bb`  
		Last Modified: Wed, 02 Feb 2022 05:08:57 GMT  
		Size: 8.6 KB (8553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a1034ed11f820e05de9c470aa0d4224878660201c2d0c743b690f478f7056f`  
		Last Modified: Wed, 02 Feb 2022 05:08:56 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48496d157566bb9ce045102b89c481cadec5104784f87402a9216ebf9579329`  
		Last Modified: Wed, 02 Feb 2022 05:09:04 GMT  
		Size: 185.1 MB (185115115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb928fe21b36d8ecceec38aae43e19dd9b26a6fe22ceb27314b243d0b0a1e803`  
		Last Modified: Wed, 02 Feb 2022 05:08:56 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07e48d708550b1a8f3d2fc1c5bafaa3844db7838117c311cd97284105edd16`  
		Last Modified: Wed, 02 Feb 2022 05:08:56 GMT  
		Size: 10.0 KB (10044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c6fae8d22548c413bb20faedcb3b30d1fade9dadc80a1da761cc412b6b22e2`  
		Last Modified: Wed, 02 Feb 2022 05:08:57 GMT  
		Size: 13.7 MB (13743117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.9-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:e14db02de6180af0f230695acf8b8e133080429b17300fce8010551f7ef7b062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.9-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:52e13f79f2905f25834fe43ff7e59346dea247dcf290f1032c8f0c3bee2b9e8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297419235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b148d4f7719405f5e8becb38ce1ea0d28eab8f249b15baac66bc04812aa69520`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:21:09 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Tue, 01 Feb 2022 02:21:52 GMT
ARG LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa
# Tue, 01 Feb 2022 02:21:52 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Tue, 01 Feb 2022 02:21:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip
# Tue, 01 Feb 2022 02:21:52 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:21:52 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:21:53 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:21:53 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:21:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Tue, 01 Feb 2022 02:21:53 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:21:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:22:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:22:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:22:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:22:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:22:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:22:38 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:22:38 GMT
USER 1001
# Tue, 01 Feb 2022 02:22:38 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:22:38 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:22:39 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22ffbf3f84215f5144dc4dba3ce08a91aee1749043f8d24b36710aa5712aa46`  
		Last Modified: Tue, 01 Feb 2022 02:27:46 GMT  
		Size: 8.6 KB (8554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10518623b1a6a24f679185c6ad9673186e493fbb180975ebe25f12223bdcda2`  
		Last Modified: Tue, 01 Feb 2022 02:27:43 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ef497ffaa162292d2461cc2df552866735173b8f20c242d2fdeaa168ff5460`  
		Last Modified: Tue, 01 Feb 2022 02:27:53 GMT  
		Size: 185.1 MB (185114875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bfd579819e102db83265151966671ce96f27e191f91e9d57a8b12292177eb2`  
		Last Modified: Tue, 01 Feb 2022 02:27:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58cb00010ac0db9ee7ca82d5b69e54ae29632ecc1d032d3dbb8d87690a5697b`  
		Last Modified: Tue, 01 Feb 2022 02:27:43 GMT  
		Size: 10.0 KB (10039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6db1c872bb7c14540b931b886412c549a5e9bd380e5369b6ce41d817b7803`  
		Last Modified: Tue, 01 Feb 2022 02:27:45 GMT  
		Size: 13.5 MB (13460537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:ad38d71918bcd430b5039aa9d47186ebc0cdbef393a03f62bf2ce6b07302d05a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301549109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c2c3645fe35ed32693ada8c9f8b66551bfd87173c378d6153b6973f375f404`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:23:45 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 14:34:39 GMT
ARG LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa
# Wed, 02 Feb 2022 14:34:44 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 14:34:54 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip
# Wed, 02 Feb 2022 14:35:07 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:35:15 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:35:21 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:35:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:35:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 14:35:41 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:35:42 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:39:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:39:13 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:39:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:39:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:40:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:40:51 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:40:56 GMT
USER 1001
# Wed, 02 Feb 2022 14:41:01 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:41:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:41:11 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fd82e0a06e099d8da55499f492a2b4e570a209af7dc2bb4d04411efdc8871a`  
		Last Modified: Wed, 02 Feb 2022 14:52:30 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322b0c658ed724950fe3f0bbc2b546d58bd7aab4caefab44fece4ddcf357f71d`  
		Last Modified: Wed, 02 Feb 2022 14:52:28 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb084f9849045b8025d4d857de8c00ac7f975b41284de3e130ddd25a47a5656a`  
		Last Modified: Wed, 02 Feb 2022 14:52:45 GMT  
		Size: 185.1 MB (185115533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0a1c1abade6d69440520243736be20b691f97ec23970e4b349898272ec172`  
		Last Modified: Wed, 02 Feb 2022 14:52:28 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e672822753d2df54087a20ddc66cd96c7bdfd72050a986ab483d3ef35577309`  
		Last Modified: Wed, 02 Feb 2022 14:52:28 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8caa119442811dcaa95a5230fbcbb144d43229cf61ff8574546395c19b1aaa`  
		Last Modified: Wed, 02 Feb 2022 14:52:30 GMT  
		Size: 12.0 MB (11992268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:7047c19c5d045665dd88fd9d00779cd770a21af688a47db8050d4fae74b29f60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.3 MB (292256118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ab3842b068800d11de1d679804311108ebd726b3c00a2951c7a1a602959206`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 05:02:54 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 05:03:38 GMT
ARG LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa
# Wed, 02 Feb 2022 05:03:38 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 05:03:38 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip
# Wed, 02 Feb 2022 05:03:39 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:03:39 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:03:39 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:03:39 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:03:39 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 05:03:39 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:03:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:03:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:03:57 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:03:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:03:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:04:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/21.0.0.9/openliberty-runtime-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=102958ae6e070c29a7b5c55b4c414953900283fa LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:04:18 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:04:18 GMT
USER 1001
# Wed, 02 Feb 2022 05:04:18 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:04:18 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:04:18 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0538fa52185763a9ddea191608682d34290e8e492324b5ac6ca0143d08dfb`  
		Last Modified: Wed, 02 Feb 2022 05:08:43 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e3dbebc55ee9019f5a1aa5d8913adb4d905f74201fd41316495151eb7d060e`  
		Last Modified: Wed, 02 Feb 2022 05:08:42 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4144d8078e42178bbc29045670deb8f3d38df9de4ffb0cd21eb7694fa6598d46`  
		Last Modified: Wed, 02 Feb 2022 05:08:51 GMT  
		Size: 185.1 MB (185115038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c504e72936e0904714d09202222d1c00db8d430228998c1cbb7a433cacc6d897`  
		Last Modified: Wed, 02 Feb 2022 05:08:42 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0beab56f8b06964512c267f7dd6ece47f9cef0ae4addbc4dbf2ae8e56f158`  
		Last Modified: Wed, 02 Feb 2022 05:08:42 GMT  
		Size: 10.0 KB (10046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160ef9187735ec653122a39df6358153f400e45ba499d7c795465ad7a849b8f`  
		Last Modified: Wed, 02 Feb 2022 05:08:43 GMT  
		Size: 10.8 MB (10762984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.9-kernel-slim-java11-openj9`

```console
$ docker pull open-liberty@sha256:71661b8c0746f7dceb35c246f7026409aafc0db75f858e2a1efc01db9d050a79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.9-kernel-slim-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:1ea2e7781dbe0c83636e5a55163f4a44f820bcfe03ae57228b8256898f545e92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ecf5b45c3f4d529a92d1c500b308197863d434a9f11cd29d0dc797555f5a104`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:21:28 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Tue, 01 Feb 2022 02:21:28 GMT
ARG LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278
# Tue, 01 Feb 2022 02:21:29 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Tue, 01 Feb 2022 02:21:29 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip
# Tue, 01 Feb 2022 02:21:29 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:21:29 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:21:29 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:21:30 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:21:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Tue, 01 Feb 2022 02:21:30 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:21:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:21:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:21:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:21:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:21:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:21:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:21:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:21:46 GMT
USER 1001
# Tue, 01 Feb 2022 02:21:46 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:21:47 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:21:47 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8241296a96b50818a496d5c58298c46aae04c3fcd18c3dc3b91fb2fe889abc9`  
		Last Modified: Tue, 01 Feb 2022 02:27:37 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0c52e818ce558cec4280459ae22f1423f44e54b092a4b0352472709bf645cc`  
		Last Modified: Tue, 01 Feb 2022 02:27:35 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39baa127e5b0692321909fe7d1da3e093653dcfd5afe1ea14c83a9d01260abe0`  
		Last Modified: Tue, 01 Feb 2022 02:27:35 GMT  
		Size: 11.8 MB (11770288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a090e8245100741746111f64da16cb6d26f4a93d5d0a15ca51766659c492b4f5`  
		Last Modified: Tue, 01 Feb 2022 02:27:34 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896a6b959352dadaac633a478d1683064bab88c8fd162cd12a6c15904f4ccb6`  
		Last Modified: Tue, 01 Feb 2022 02:27:34 GMT  
		Size: 9.2 KB (9213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33640980e88fb99a1e82b32a40ba7c1e0fc05adb505742ac5c19c63cc1013382`  
		Last Modified: Tue, 01 Feb 2022 02:27:35 GMT  
		Size: 2.5 MB (2524350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-kernel-slim-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:38041ba2d594dd4d9604b2d37422f7c68525a31d668d38f36c24084d5084fdfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116396433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a5c078e9d3d195af07999001da4018aeff9fbe88210247a78b5c86ae9a95a5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:27:58 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 14:28:03 GMT
ARG LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278
# Wed, 02 Feb 2022 14:28:08 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 14:28:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip
# Wed, 02 Feb 2022 14:28:16 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:28:21 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:28:25 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:28:30 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:28:36 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 14:28:41 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:28:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:33:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:33:04 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:33:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:33:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:34:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:34:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:34:13 GMT
USER 1001
# Wed, 02 Feb 2022 14:34:17 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:34:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:34:27 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d14ee8d07a25870123d67ba1b59d0af548ae9468c1924cb4aa93c411250a274`  
		Last Modified: Wed, 02 Feb 2022 14:52:20 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad38cf5b707e54182328ce7ab6c22e065343108d4cb2ae6f66e6840aa8273a`  
		Last Modified: Wed, 02 Feb 2022 14:52:17 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fa8fea6830af0b55b241b720c2d88da29a69d618981ecf06efdbb7f7e75d2`  
		Last Modified: Wed, 02 Feb 2022 14:52:19 GMT  
		Size: 11.8 MB (11771026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e2e5da79fe647572eb2b348d901b1404a7603df71957ef3fff4ee426fb58f1`  
		Last Modified: Wed, 02 Feb 2022 14:52:17 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db07d99abd8a0f0b9e788e480f230c53ec030470cc81dc552ed8212be6e46d06`  
		Last Modified: Wed, 02 Feb 2022 14:52:17 GMT  
		Size: 9.2 KB (9241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05247ab36dc184576cc605dda2c6b35ceb25c77bff01735f17d2b0670bf18f5d`  
		Last Modified: Wed, 02 Feb 2022 14:52:18 GMT  
		Size: 2.4 MB (2441818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-kernel-slim-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:d56dbcca48487f1576690e0bd7816a076f9147a5ee0a16bff6e9ceb01dc19dfb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108093441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310b1dd2719665e81a5f8623be18e995f9fae126e0286a26a2b874585c9b9147`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 05:03:16 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 05:03:16 GMT
ARG LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278
# Wed, 02 Feb 2022 05:03:17 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 05:03:17 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip
# Wed, 02 Feb 2022 05:03:17 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:03:17 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:03:17 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:03:17 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:03:17 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 05:03:18 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:03:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:03:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:03:24 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:03:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:03:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:03:31 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:03:31 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:03:31 GMT
USER 1001
# Wed, 02 Feb 2022 05:03:32 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:03:32 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:03:32 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a100f174148fc3552342bbd93df5b053799dbe8794689f70d68eca80df41500`  
		Last Modified: Wed, 02 Feb 2022 05:08:37 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bcff276201e6217ab1f37c0f4419ca8dc6a5092db4860f5aba2a36d7a9c410`  
		Last Modified: Wed, 02 Feb 2022 05:08:36 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7ce6490852ff4a26a4bdee0a83494889514021b0f2cb74d80081ae22969da6`  
		Last Modified: Wed, 02 Feb 2022 05:08:37 GMT  
		Size: 11.8 MB (11770566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afea8e11bd048a7e21ca9f9854f0845d84e1adf6757b1b491c4dafb6faf4fd14`  
		Last Modified: Wed, 02 Feb 2022 05:08:36 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e853a5d885ce68ac8e25fea7c8db06c6e95172d80b958adf5817f6718481c`  
		Last Modified: Wed, 02 Feb 2022 05:08:36 GMT  
		Size: 9.2 KB (9209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a0be46e8383af8accefaed6a4b9a8ed5f6c97750322447b869a05250a1fb11`  
		Last Modified: Wed, 02 Feb 2022 05:08:37 GMT  
		Size: 2.5 MB (2473784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:21.0.0.9-kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:a286aaaa8095c783f603a6b336b8422d7cca62515015064306928e6d90a3ea82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:21.0.0.9-kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:d44ae33972dd1fef8a4386b8183648b9c6378e14c4680302c563dd245220d32f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113067386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af054f8d3314da447ecf4af159adfaacd907f20f4bbef200419d1d893d6c134f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:21:09 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Tue, 01 Feb 2022 02:21:09 GMT
ARG LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278
# Tue, 01 Feb 2022 02:21:09 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Tue, 01 Feb 2022 02:21:09 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip
# Tue, 01 Feb 2022 02:21:10 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:21:10 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:21:10 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:21:10 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:21:10 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Tue, 01 Feb 2022 02:21:11 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:21:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:21:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:21:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:21:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:21:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:21:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:21:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:21:25 GMT
USER 1001
# Tue, 01 Feb 2022 02:21:26 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:21:26 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:21:26 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e571a091ebb71124666fcdbe8bf59bbabe8cfee1f0881800f8e7d6133b722ca7`  
		Last Modified: Tue, 01 Feb 2022 02:27:28 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfba77e4e695b32f39218d1777afd2a939ce7716f99470a83fd621658633e124`  
		Last Modified: Tue, 01 Feb 2022 02:27:26 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d0355d24ee700e8242e0cebc11e4c03c1e13e5e022bd4e74ba682b2fc2da9`  
		Last Modified: Tue, 01 Feb 2022 02:27:27 GMT  
		Size: 11.8 MB (11770327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79e5aff74779fcd1d50b4259e9149696cfd1378722fa5aab0cc0d429472a7dd`  
		Last Modified: Tue, 01 Feb 2022 02:27:26 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afd96c3a0faa82d78e3bec93ff5c72d8ea386425c7b4cfb1629493c95834faf`  
		Last Modified: Tue, 01 Feb 2022 02:27:26 GMT  
		Size: 9.2 KB (9217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae1c95aa827493b84a8f61f5cc049c584ca2ee7cb8b397343edc9ec4d03793a`  
		Last Modified: Tue, 01 Feb 2022 02:27:26 GMT  
		Size: 2.5 MB (2454822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:3cc31111c83fbe9d17056f69e02dfe8a6a18ea805854ac9998d043c130e701b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118629105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dd0681364d0f66cb0adb67966364c2fee2bdce93fc6cb3a60ad6ee732c2f5d7`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 14:23:45 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 14:23:50 GMT
ARG LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278
# Wed, 02 Feb 2022 14:24:00 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 14:24:06 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip
# Wed, 02 Feb 2022 14:24:10 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 14:24:13 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 14:24:17 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:24:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 14:24:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 14:24:28 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 14:24:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:26:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:26:17 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:26:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:26:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:27:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:27:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:27:24 GMT
USER 1001
# Wed, 02 Feb 2022 14:27:29 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:27:33 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:27:40 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b8f581305e882e2a712bfb417d353241c26842c5772d924243a2704843d96f`  
		Last Modified: Wed, 02 Feb 2022 14:52:09 GMT  
		Size: 8.1 KB (8114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715facebba8b4d04b02a76203eea72828f1d21b094c9d862c8287ae39e33fb99`  
		Last Modified: Wed, 02 Feb 2022 14:52:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a98f5bbcbce745154cccb9c9d9c3a05efc003bf6195b8dd475fef5c46676e8a`  
		Last Modified: Wed, 02 Feb 2022 14:52:06 GMT  
		Size: 11.8 MB (11771011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45b03db3a85fbe7e5b5cd3aebfea4080e05c85a34641303c4489ac04ca3b1c6`  
		Last Modified: Wed, 02 Feb 2022 14:52:05 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef9e9799419a0f54478fd2abd6ee72ea23ba43319285a34fbaed029d4992580`  
		Last Modified: Wed, 02 Feb 2022 14:52:05 GMT  
		Size: 9.2 KB (9238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b22863fbab8506903562520598c895a67f70754a23eada5013a3d5bb4a1ceb7`  
		Last Modified: Wed, 02 Feb 2022 14:52:06 GMT  
		Size: 2.4 MB (2418370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:21.0.0.9-kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:aaa749d1ef3a5468b9f0949501391bd6ae2044450d25660e78e702e89d7afa9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110392076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebfc760bfb43241c50023483d9b9a4e6f17a70a326ef7b133c6facfbb0926be0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 05:02:54 GMT
ARG LIBERTY_VERSION=21.0.0.9
# Wed, 02 Feb 2022 05:02:54 GMT
ARG LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278
# Wed, 02 Feb 2022 05:02:54 GMT
ARG LIBERTY_BUILD_LABEL=cl210920210824-2341
# Wed, 02 Feb 2022 05:02:54 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip
# Wed, 02 Feb 2022 05:02:55 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 05:02:55 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 05:02:55 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:02:55 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:02:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=21.0.0.9
# Wed, 02 Feb 2022 05:02:55 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 05:02:55 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 05:03:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 05:03:01 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:03:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:03:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 05:03:08 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl210920210824-2341 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/21.0.0.9/openliberty-kernel-21.0.0.9.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=82894898cdb1824d173c3e87052f93230c163278 LIBERTY_VERSION=21.0.0.9 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 05:03:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:03:08 GMT
USER 1001
# Wed, 02 Feb 2022 05:03:08 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:03:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:03:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7ab35a639a333373aeefba511e7357e93c396f042d009e50695fd09c3ef016`  
		Last Modified: Wed, 02 Feb 2022 05:08:31 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1521638cdc069d7c005f9edbcfd81116de56abb7852b7414244a075a1b1cd67a`  
		Last Modified: Wed, 02 Feb 2022 05:08:30 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea607b8eefcef3b702b52cfb8980f5c0d880b5ec25071d27203deeb06850e9`  
		Last Modified: Wed, 02 Feb 2022 05:08:30 GMT  
		Size: 11.8 MB (11770536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50560763acfae66cffd48e117f5ab7aca66351f7d88f5c6ac90fdfdc9a181ca2`  
		Last Modified: Wed, 02 Feb 2022 05:08:30 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7610c0c7370b7653abcfebae077675d84df3c79dbd702d5cc0bd0349b695f59d`  
		Last Modified: Wed, 02 Feb 2022 05:08:30 GMT  
		Size: 9.2 KB (9212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc4343a018b9f59440f3195ca1b4d7139b2b7c7c8529752c51395f58a36b953`  
		Last Modified: Wed, 02 Feb 2022 05:08:30 GMT  
		Size: 2.2 MB (2245038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:22.0.0.1-full-java11-openj9`

```console
$ docker pull open-liberty@sha256:0618eca4d60a4cf43ab63ad949f2c8270a27592c9d91059d218d85d8a27aca3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:22.0.0.1-full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:56e6dbb0f19e2dc6a2a2bf15cd7824b4abaa6aa7327944cd265c33fb0e980f1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.3 MB (402259935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc588c675c48e3272cad11bb260bfb2edffde6824a252a33a0221258e49b8c6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:17:27 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:17:27 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:17:27 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:17:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:17:27 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:17:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:17:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:17:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:17:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:17:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:18:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:18:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:18:16 GMT
USER 1001
# Tue, 01 Feb 2022 02:18:17 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:18:17 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:18:17 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502e7c64d459bd6cede5f1840b31534d4779e09fbcb65e2f9be1de2559f0a547`  
		Last Modified: Tue, 01 Feb 2022 02:25:53 GMT  
		Size: 8.6 KB (8550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a4ceef09c7c59993174e959a8c5e3abb92de69c67ae653181d4abbcc7b4319`  
		Last Modified: Tue, 01 Feb 2022 02:25:51 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2414052f962e781be1fc6a8b106e8c72454a9c648802ff5cbfa8cba5f8674179`  
		Last Modified: Tue, 01 Feb 2022 02:26:05 GMT  
		Size: 291.7 MB (291675754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ba754a35e035fe07a08616849f23364616b387b6c77dacba1e55e53e6d812`  
		Last Modified: Tue, 01 Feb 2022 02:25:51 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370d7762a1d46c1b36eeb7e9dc34daa38f957765fc1366e872fc3d1dc898ec5b`  
		Last Modified: Tue, 01 Feb 2022 02:25:51 GMT  
		Size: 10.0 KB (10042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d33103a128c06253c47add0ba6a3294ed03b45ffa95ca6de1eaafa1dd5aadf8`  
		Last Modified: Tue, 01 Feb 2022 02:25:54 GMT  
		Size: 13.9 MB (13850194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b00bde9f06f57a1270f322ccd68a6da67f29d2352ac5698b02cd738b8f6098b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.1 MB (406084445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923cb9479651dadb1e85e2bcbff89dc395232cc5443d36fcd04f0ad24d9670d2`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:49:09 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:56:30 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 13:56:32 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:56:34 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 13:56:35 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:56:37 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:56:39 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:56:41 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:56:43 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:56:44 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:56:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:02:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:03:08 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:03:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:03:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:04:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:04:44 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:04:48 GMT
USER 1001
# Wed, 02 Feb 2022 14:04:51 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:04:56 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:04:59 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd519597fe72ce8b1344442be07458ad187acc1b64dbb8a8183487f749c3bbf1`  
		Last Modified: Wed, 02 Feb 2022 14:49:43 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4202f45c2725044fd3f9e269949a6abfc301d68711cde295b94430c51fd8d91`  
		Last Modified: Wed, 02 Feb 2022 14:49:40 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd99c0f2987d13cbaac5c80c3c8458227142ab88eed8a5302be3310cefa109`  
		Last Modified: Wed, 02 Feb 2022 14:50:10 GMT  
		Size: 291.7 MB (291676319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbaa8ff22cc19a669b732bc3738ce13926e7a7a8afb984f50bf842fe65a852a`  
		Last Modified: Wed, 02 Feb 2022 14:49:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb7bb68083573cc3090729eab966810568d852124913ca1fde3149f5fd7e8e`  
		Last Modified: Wed, 02 Feb 2022 14:49:40 GMT  
		Size: 10.1 KB (10067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347d59b924351befed80c43cc6ad75ce4c6ff319cec64482eb23663a83c9ec11`  
		Last Modified: Wed, 02 Feb 2022 14:49:42 GMT  
		Size: 12.2 MB (12222949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:ec184e4c286813121b2577b305751a63e2051fa172a626acb753a3d5960810e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.4 MB (399367610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427e39802d3664950186cc709ca9c13969ff56d94458609dd53e78f2824e050b`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:55:32 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:56:54 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:56:55 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:56:55 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:56:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:56:55 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:56:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:58:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:58:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:58:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:58:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:58:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:58:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:58:27 GMT
USER 1001
# Wed, 02 Feb 2022 04:58:28 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:58:28 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:58:28 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b28a68eb26051df97c041b172e6d74d5ae5492b9a4bcea81c1864a715684c4`  
		Last Modified: Wed, 02 Feb 2022 05:07:21 GMT  
		Size: 8.5 KB (8546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73815e61f4386b4fb2ac962fd030d492696944cb09fcdbdc4df77b330aa2af`  
		Last Modified: Wed, 02 Feb 2022 05:07:20 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30796d6efd8445365a3305a06c487082d82c3818a46b57cf03dee4c44c6a8718`  
		Last Modified: Wed, 02 Feb 2022 05:07:32 GMT  
		Size: 291.7 MB (291675973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d176335a99e00c1470f24b01881466ed7637c4d657bf693f3258836a4b91a43`  
		Last Modified: Wed, 02 Feb 2022 05:07:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1797525c5fbb7f0a412d0862ffddd68c605975b9e863a0499a246b71695ed2`  
		Last Modified: Wed, 02 Feb 2022 05:07:20 GMT  
		Size: 10.0 KB (10041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dacfbdebf94b1dc6f136bf8c17218209e5885b9c311a6687b300a40337e12bf`  
		Last Modified: Wed, 02 Feb 2022 05:07:21 GMT  
		Size: 13.8 MB (13840963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:22.0.0.1-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:0f169a11e9f2ece11364f95981929068c575c908fa4b78a4edaad5d796ea9c50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:22.0.0.1-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:d765a38c29f93b182c2ad64252826f928d1e2388014a4375936f2ac1e6fe806c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.1 MB (404055676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4363749360ffcb5d9356a2d92c680c8bef4c59cc5bd68de98c7048ddcaa3d219`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:16:04 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:04 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:16:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:16:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:16:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:16:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:17:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:17:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:17:14 GMT
USER 1001
# Tue, 01 Feb 2022 02:17:14 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:17:14 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:17:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0dd06f22af6d321debcc35fe49584e9508f3f8a9a34c9529a161d3b1d5859`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d871f90dc74ad1930ad07a28487c241564a95b4c2c807fa7498d7e6a00f071`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab0cd22ea6a2058ef644493e80d0144abf96f82cc9eb6268ff21383e96b39ad`  
		Last Modified: Tue, 01 Feb 2022 02:25:39 GMT  
		Size: 291.7 MB (291675718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb30f069fa13018d762521188faf3f255a2d9e2044dd45b46b39153623d89baa`  
		Last Modified: Tue, 01 Feb 2022 02:25:26 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c30df76bf4c02eaca50fee021d65c4d53ece95d36e1f22ebec0300d997b3102`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 10.1 KB (10052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22256b7cdc0b66dd775f30efcc4196b11b13ce4636d0b4bb4fcac17465b27d72`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 13.5 MB (13536116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:c37ba13362eed0a493c3e89984e50783f28f9e9e4a3a01bf3cab14119da1243c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.2 MB (408174413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a30cf262b777ee5a509f742afd88c46e29562fc9340f27cd185bb1de972d97d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:52:34 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 13:52:37 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:52:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 13:52:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:52:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:52:49 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:52:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:52:53 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:52:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:55:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:55:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:55:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:55:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:56:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:56:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:56:16 GMT
USER 1001
# Wed, 02 Feb 2022 13:56:17 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:56:20 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:56:22 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ec8b529c9dfc92f266863cb3cab0c9cabae82b6054a5ab6a102412d3d5c05`  
		Last Modified: Wed, 02 Feb 2022 14:48:57 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d314dc71e6bdf9b22e3000713842dfa6f7626239b3c3ffe91fce14937932fca`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0438eb8384253339c23764c856a2d4b4760d5cf877831869a445d300a612b`  
		Last Modified: Wed, 02 Feb 2022 14:49:20 GMT  
		Size: 291.7 MB (291676389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fdf6c1b7f149ace90882402b18a91bfb0f339f36ef947ba9e7a3d85d4f4a`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a1499353c85e51e33a6022fd6b6292d73d47bb334490c6444e464eb15f866f`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8db058827844fcef088df1ddeed8a6cebcf21d5add3cc4cb95cd3e16799756`  
		Last Modified: Wed, 02 Feb 2022 14:48:56 GMT  
		Size: 12.1 MB (12056712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:38ff00003cb886c8c096f1c2df08190807a59a10267c3796c49f471244ba0d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.9 MB (398879420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae86a30a90c24730c99c856a42bfecc96cea509d841bee1bd9b27b9da5e4622d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:55:58 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:55:58 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:58 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:55:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:55:58 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:55:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:56:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:56:25 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:56:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:56:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:56:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:56:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:56:46 GMT
USER 1001
# Wed, 02 Feb 2022 04:56:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:56:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:56:46 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3be9e00dbaa95dc5001e009e4a48f7bcb181012da6bcfbacd3faee29960d4e`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9128b48078d3a8f12b88808347a020a7df9f52091f1350c33a5c576d5bb665`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e5eb7eb37b3a087d8338dc2517841b9eaf4a37e546248bf50611c3fd162f76`  
		Last Modified: Wed, 02 Feb 2022 05:07:10 GMT  
		Size: 291.7 MB (291675971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ec240b69b0c5e711e0e971ace42fed0d4b1571aca08c322bb3829faf44c8b4`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bef308e4d233fd0433437d8949545adfdc3f22735b8a89def423c0b3204d08`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 10.0 KB (10043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc63c160bc902af47a99874236ba953f3cd6e49b192c16c0b1ab97881fd47f9b`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 10.8 MB (10825360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:22.0.0.1-kernel-slim-java11-openj9`

```console
$ docker pull open-liberty@sha256:368eb70918ec75b0c7188eac8eda14ea184613e778dc2185818ee9bdfead8ebb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:22.0.0.1-kernel-slim-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:5f930e67e211063a5947a13d25f8814b4820e0cc2a7d723b7d4186b1d8014c1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111003271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435d4b0d4a8948c126cc5f8c2f82142019407e21797ec221e4b10724ab88ac24`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Tue, 01 Feb 2022 02:15:41 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:15:41 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:15:41 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:41 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:15:41 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:15:42 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:15:42 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:15:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:15:47 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:15:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:15:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:15:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:15:57 GMT
USER 1001
# Tue, 01 Feb 2022 02:15:57 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:15:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:15:58 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ad96cb23fd36be631079e155934175b17d24fab63cdf253ef96d530e597af`  
		Last Modified: Tue, 01 Feb 2022 02:25:18 GMT  
		Size: 8.1 KB (8112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebc94632c966c3394394e1eee7b98294808a90fa5111425a2f12cd0faa09bf5`  
		Last Modified: Tue, 01 Feb 2022 02:25:16 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c807b8634aa793a3eb773f15c494e35eece09b87817ee6a454df02bbc2a32687`  
		Last Modified: Tue, 01 Feb 2022 02:25:17 GMT  
		Size: 11.8 MB (11814321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6014a014aeb2d7275c8be20d69db6735e8e2c31aaadb00cc72b7574d951673d`  
		Last Modified: Tue, 01 Feb 2022 02:25:16 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a069f334ed8c9cbda175ab76a832c4eadfd6d07543581b4e7c21a2d7deb6185`  
		Last Modified: Tue, 01 Feb 2022 02:25:17 GMT  
		Size: 9.2 KB (9222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8882a6d4d985523ebab8a95360e1dcdfd2f97e5ef3633376f79b5f32cdb12`  
		Last Modified: Tue, 01 Feb 2022 02:25:16 GMT  
		Size: 2.5 MB (2456554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-kernel-slim-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:9d789995f5a4176331fb218d86c2710a3e401f904c0e96e136fc2b6af3700041
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116433217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb3e7377f72980e4b12a8234a3e958c425ce253fa7a65e96f7ef76d10913e36`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:49:09 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:49:12 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 13:49:14 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:49:15 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 13:49:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:49:20 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:49:24 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:49:26 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:49:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:49:32 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:49:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:51:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:51:24 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:51:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:51:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:52:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:52:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:52:11 GMT
USER 1001
# Wed, 02 Feb 2022 13:52:15 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:52:16 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:52:20 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872852080f61b21851572b031d3eef74ac2eed627323c0be7936c9029e1b9b5`  
		Last Modified: Wed, 02 Feb 2022 14:48:45 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd8a421d5324e1d3cd3379bc54bcf2cd07fdd1b8acc576b5ccb2ae3d824e42e`  
		Last Modified: Wed, 02 Feb 2022 14:48:42 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b59ffab32c7a4660da62455898e020beb97ac6c59848b9898c4a3a0a5a9a84d`  
		Last Modified: Wed, 02 Feb 2022 14:48:43 GMT  
		Size: 11.8 MB (11814988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c721178cfe52334d7354db94a334c24322e6082478096d5599a66714331bf65`  
		Last Modified: Wed, 02 Feb 2022 14:48:42 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43cd69d36c3f095cecf827cb691d95ff30003a50312860be68259e56b8954d`  
		Last Modified: Wed, 02 Feb 2022 14:48:42 GMT  
		Size: 9.2 KB (9235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4af65f391d30393f64b1fb0659065b4717f2bc51a50ab7ffb2ffb99274281f`  
		Last Modified: Wed, 02 Feb 2022 14:48:43 GMT  
		Size: 2.4 MB (2434644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-kernel-slim-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:42b1100930cc8f72129d9f419f732692597f4d374dc665b89ed7509b76c3b64b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108136071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99dae7bcc64140db9458f25eacb72497b5477df1b9122b3cd89df1d12fb2ec17`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:55:32 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:55:32 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:55:33 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:33 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:55:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:55:34 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:55:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:55:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:55:42 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:55:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:55:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:55:49 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:55:49 GMT
USER 1001
# Wed, 02 Feb 2022 04:55:49 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:55:49 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:55:49 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529b12ae434e8444f3f02fac8a9ea9bfa3b593462e008d2eaa1b53168d2ff808`  
		Last Modified: Wed, 02 Feb 2022 05:06:54 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e8f07cb58b2bafceaf238d7823cdf81f79d182ad8155b1a2c8220f2b73a26a`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36adbade8d4ef4a2f5441b06bc817a666fb690fb34a471740da6139d76f6bf20`  
		Last Modified: Wed, 02 Feb 2022 05:06:54 GMT  
		Size: 11.8 MB (11814539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9907e3b73349d5b48d31826024581694319df42403bcf4f2c74993e7157f0529`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f005f776114fec1122eef836d55dd09deb87c6fc367470bf77eb22255cc470ff`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 9.2 KB (9213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7f5aaed942ab6af3b8e2dd2b26439d8c5978259dc806572f3235c20e1bb8`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 2.5 MB (2472444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:22.0.0.1-kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:b02e7de7e19bb016efaf082af181c3ba3678b807ae993830899fd519a77c59e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:22.0.0.1-kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:331e97c4e89399cfaa922e66788752932dd920d11c21476ba2874633e0a09525
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113096280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adbc584c36ae3c4eab850f94fcb0dd9ad46784ae4f0050f0bd5ed1dc0f21c80e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:15:22 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:22 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:15:22 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:15:22 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:15:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:15:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:15:28 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:15:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:15:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:15:37 GMT
USER 1001
# Tue, 01 Feb 2022 02:15:37 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:15:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:15:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdca4a06ca8bdadbdfced7e1e293379dfa19d8c6267d805bd23cceeb7b4f28a`  
		Last Modified: Tue, 01 Feb 2022 02:25:06 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915ee96ab3c294a6cebf8f011b1d6c832a87073596878d8bb438a243ec24fb28`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e881d56be87250c1d78d22954a8a10c6db9aa7fe53e830a923ff1ac9cd0a0a85`  
		Last Modified: Tue, 01 Feb 2022 02:25:05 GMT  
		Size: 11.8 MB (11814321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf9961f6b52f2af462e9ad187230136d1c92cc2e676edbcb3281d355f72f72`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f112feffa1f30cf33f0988bd507269849e1ad1e1ce9c700ae08d556e720707`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 9.2 KB (9211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e412099596dad8b30bb0704bb2812daf9535e73de582880fa415e84f8a2b748`  
		Last Modified: Tue, 01 Feb 2022 02:25:05 GMT  
		Size: 2.4 MB (2439725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:95dc78c596863727e7e53f9e3a869f4f3dce720385ae70cf58f54dfce85f69cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118667124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd88fd7312cb7cba7b1001eb57aefeb6b2e09bc1d4082d102066851702a66cb5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:45:31 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 13:45:35 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:45:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 13:45:41 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:45:43 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:45:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:45:48 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:45:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:45:51 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:45:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:48:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:48:19 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:48:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:48:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:48:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:48:53 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:48:56 GMT
USER 1001
# Wed, 02 Feb 2022 13:48:57 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:48:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:49:01 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b9604213edbe2684cacee5c5d17ff9922642da340455dacb9fb7079e5f5442`  
		Last Modified: Wed, 02 Feb 2022 14:48:28 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35fcc8a334d355228479a7b9f29038bbd05e7fa176b00289b25e900343d9fab`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ddb0cab9d3f827f351bfe1c1e251a7ba45a4b75542c906b5ea0ab2321577f`  
		Last Modified: Wed, 02 Feb 2022 14:48:27 GMT  
		Size: 11.8 MB (11815006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf24a37641ad7ae733bb4c1ef9f67a5e8044fa1720d665f71013d9be824ab5c2`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c472c2f1ff5cd1610a38158f47f53b6618efc7cc3625bd66e94e05eb46e9845`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 9.2 KB (9240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aff7a56991fd0349ecd9980c613d57a6c20786f91bdeab5a6fa73a4d0b1c5e5`  
		Last Modified: Wed, 02 Feb 2022 14:48:25 GMT  
		Size: 2.4 MB (2412396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:22.0.0.1-kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:6a02f53d7133be6696647095385a6f0206abe3b60d70d4904e329fc1e5b70ce1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110433107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01a915d38097f490c316613b2d1f86e23ac1822790f90e9278d1bb4d808ac40c`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:54:25 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:54:25 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:54:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:54:26 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:54:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:55:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:55:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:55:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:55:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:55:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:55:25 GMT
USER 1001
# Wed, 02 Feb 2022 04:55:25 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:55:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:55:25 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae67e91b406ba6c368b5cf5e1d449b3d23ec4d15803d2c72d7c6a128d7103e63`  
		Last Modified: Wed, 02 Feb 2022 05:06:46 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2684cfa6bf38124a704e6111da0a41c4b3fa4fa2738734f8f3151263b86cc89a`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da325492888060446c03d0332f5cf21f4e89b29ef0d229ea913a10879418bcb9`  
		Last Modified: Wed, 02 Feb 2022 05:06:46 GMT  
		Size: 11.8 MB (11814528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95fac8ac0494f895f01fe281e4c8dddd12a382e8d4332723af592d36aaed758`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ed72f7e97cc70a57c36cd0124a7e7fa863a7fb62d8c94b3bcb35ae300d88be`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 9.2 KB (9219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c00e6613a88743d6bd75a56a43d670fdea29658113e6348ad3782760f818367`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 2.2 MB (2242073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:beta`

```console
$ docker pull open-liberty@sha256:95ac779a1c87517466212c29c8412b9d0a2a3564e68c6fb3afd1f78e43c3359a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta` - linux; amd64

```console
$ docker pull open-liberty@sha256:9a33148030a542a3a93fa84a8c69551bb9ac49c101e6479fde9e8ef959c5344a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.8 MB (412797316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41982b48f990707851e59646b3859114d1f0bf287d4114c210f8b85bb0377183`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:13:14 GMT
ARG LIBERTY_VERSION=22.0.0.2-beta
# Tue, 01 Feb 2022 02:13:14 GMT
ARG LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8
# Tue, 01 Feb 2022 02:13:14 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:13:14 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip
# Tue, 01 Feb 2022 02:13:15 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:13:15 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:13:15 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:13:15 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:13:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 8 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.2-beta
# Tue, 01 Feb 2022 02:13:16 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:13:16 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:13:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:13:45 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:13:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:13:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:14:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:14:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:14:17 GMT
USER 1001
# Tue, 01 Feb 2022 02:14:18 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:14:18 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:14:18 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f475f888d1a071c0bcfafd36bc099da77a0437684d099877d468a180f3bb0779`  
		Last Modified: Tue, 01 Feb 2022 02:24:22 GMT  
		Size: 8.5 KB (8548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88002671653b98f4b775ff84b8e0c7d291bef81b28490e41a42527af9f29c552`  
		Last Modified: Tue, 01 Feb 2022 02:24:20 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f90ce8c5f7f102d862a558b58a441e50bbd1d3b75f00114711ce6ab40c441e3`  
		Last Modified: Tue, 01 Feb 2022 02:24:34 GMT  
		Size: 300.5 MB (300487697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef85663b52a908391c111d54a038aa5363db7a81c103e24743faabc6324911e`  
		Last Modified: Tue, 01 Feb 2022 02:24:20 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91963d040e146b4b237c4dd36687fe81dfd034ee5df3d75c78adb60878e8c3db`  
		Last Modified: Tue, 01 Feb 2022 02:24:20 GMT  
		Size: 10.1 KB (10051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a4206c8c13c0437f42e23575e20a89a3d7920f63ad0937972f617c069fb706`  
		Last Modified: Tue, 01 Feb 2022 02:24:22 GMT  
		Size: 13.5 MB (13465786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:a78eab4c8dc0a00636f35c5d13ff88560186366944aa099f6073caac4b3b686d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.0 MB (416989322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a393b3f89d7b9ff0585968ddb1fbe5dab7c017fe36d842479736c9a76c30a78`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:36:23 GMT
ARG LIBERTY_VERSION=22.0.0.2-beta
# Wed, 02 Feb 2022 13:36:25 GMT
ARG LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8
# Wed, 02 Feb 2022 13:36:30 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:36:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip
# Wed, 02 Feb 2022 13:36:36 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:36:38 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:36:40 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:36:42 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:36:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 8 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.2-beta
# Wed, 02 Feb 2022 13:36:45 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:36:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:39:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:39:43 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:39:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:40:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:40:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:40:56 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:40:58 GMT
USER 1001
# Wed, 02 Feb 2022 13:41:00 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:41:01 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:41:03 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c40407a0b6b6e9c3ed252b0673ae70a1d3bd1a3a62b69ea4bf50e98311640`  
		Last Modified: Wed, 02 Feb 2022 14:47:16 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7eeda9c587eb3bd94e14e6966580ed47231f44361db2ecfd8c1c43f65a1ee`  
		Last Modified: Wed, 02 Feb 2022 14:47:13 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048ad3c8629fe2444aa585397e038822bf47fa48cd154e2c4ee7bd30b6e6618`  
		Last Modified: Wed, 02 Feb 2022 14:47:40 GMT  
		Size: 300.5 MB (300488384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b5e2c609ee3c3fd3e26623f434217aed6f1fd99eae32107c37312ddc3be53`  
		Last Modified: Wed, 02 Feb 2022 14:47:13 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9618ac7288f67c3ddafeac3110ad16af95ab426a2baec6d1ab71a49f62113707`  
		Last Modified: Wed, 02 Feb 2022 14:47:13 GMT  
		Size: 10.1 KB (10065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f05f55ace9d0bfc65b2896a5cc4944447e6d104f85fe4f589ef229a35cb695`  
		Last Modified: Wed, 02 Feb 2022 14:47:15 GMT  
		Size: 12.1 MB (12059627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta` - linux; s390x

```console
$ docker pull open-liberty@sha256:f89c214c1c12ae3d593c18a396564533c49905780a0e847ac49da2a88ce918d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.7 MB (407692034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de7f3194fad0116efa873e09b3f8ca51a3823e2e22700f2061dd41f4b8f0778f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:51:31 GMT
ARG LIBERTY_VERSION=22.0.0.2-beta
# Wed, 02 Feb 2022 04:51:31 GMT
ARG LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8
# Wed, 02 Feb 2022 04:51:32 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:51:32 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip
# Wed, 02 Feb 2022 04:51:32 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:51:32 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:51:32 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:51:32 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:51:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 8 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.2-beta
# Wed, 02 Feb 2022 04:51:33 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:51:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:52:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:52:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:52:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:52:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:52:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:52:37 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:52:37 GMT
USER 1001
# Wed, 02 Feb 2022 04:52:37 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:52:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:52:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbddd23ab470751205ba6163da11bc36bc2c669f720aa04d9030bf23086bace8`  
		Last Modified: Wed, 02 Feb 2022 05:06:11 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0d5437cbd9dd5eed1947ef17394cc4ac8f14233ed5e603981da08d91b8cb10`  
		Last Modified: Wed, 02 Feb 2022 05:06:09 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b398b17c79d1574f5ff147e1424f6caa443f30ecf95cb0b440e1bf37f6099827`  
		Last Modified: Wed, 02 Feb 2022 05:06:22 GMT  
		Size: 300.5 MB (300487915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb7ada6bea3064388a7e88066ea3401e1374fc38cc70181d259e6a652121808`  
		Last Modified: Wed, 02 Feb 2022 05:06:09 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abff290f2ff0b28632f98ec7842ee030596001084416107e2c66f38e03d4a6f`  
		Last Modified: Wed, 02 Feb 2022 05:06:10 GMT  
		Size: 10.0 KB (10042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd74c3e5c78462fc7567b33bb523e5a07f2d7fd1d25bf164a8c76a8b64f05c6f`  
		Last Modified: Wed, 02 Feb 2022 05:06:11 GMT  
		Size: 10.8 MB (10826032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:beta-java11`

```console
$ docker pull open-liberty@sha256:11f68ea677b9bafadf0c70cac8759e3af204cdd323d320545ab3282d4b5c1137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta-java11` - linux; amd64

```console
$ docker pull open-liberty@sha256:1bc488404cac1c7c80bf69cfad9bba5ce7bc9f4641fc8533271139a488fd0395
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.2 MB (411218090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c35cc244756dea0de741cbaff6e1bce15d864e2085b46983229218b9705c30a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:14:23 GMT
ARG LIBERTY_VERSION=22.0.0.2-beta
# Tue, 01 Feb 2022 02:14:23 GMT
ARG LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8
# Tue, 01 Feb 2022 02:14:23 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:14:23 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip
# Tue, 01 Feb 2022 02:14:24 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:14:24 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:14:24 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:14:24 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:14:24 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.2-beta
# Tue, 01 Feb 2022 02:14:25 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:14:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:14:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:14:39 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:14:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:14:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:15:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:15:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:15:14 GMT
USER 1001
# Tue, 01 Feb 2022 02:15:14 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:15:14 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:15:15 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de770c0beaff95faeb01a67c8c6a386d6dbccecb42a4e47acae88ce39db3dc55`  
		Last Modified: Tue, 01 Feb 2022 02:24:45 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0448511de572943a9ceacab687450f4a47cf7c7e05a98de95cd6d1421374147`  
		Last Modified: Tue, 01 Feb 2022 02:24:42 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9d8d53c2b8d59b1040901750fe54b7623c580245271237c3cbe813231a0d58`  
		Last Modified: Tue, 01 Feb 2022 02:24:57 GMT  
		Size: 300.5 MB (300487752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e14a43cfee8a88012b3ce68ecc4af06868e45394e9d9a81715720049726e497`  
		Last Modified: Tue, 01 Feb 2022 02:24:43 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781845fabef2cb2e93f8618551943efa5c9de4f293cef5e73c850c1f83cc8865`  
		Last Modified: Tue, 01 Feb 2022 02:24:42 GMT  
		Size: 10.0 KB (10049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbf9c110b288469ee6b8244caf5b920a3474a989a42345a2719313a992f8555`  
		Last Modified: Tue, 01 Feb 2022 02:24:45 GMT  
		Size: 14.0 MB (13996343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:a3b92cd593a1b28464566d839c6f5b9e38f4ec65b4c2d78c4f2166beacc65d8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.9 MB (414880206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc853e9726986f4ccf63034cfee676c8351f115d27e5285b5244ac5ce954e594`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:41:17 GMT
ARG LIBERTY_VERSION=22.0.0.2-beta
# Wed, 02 Feb 2022 13:41:20 GMT
ARG LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8
# Wed, 02 Feb 2022 13:41:22 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:41:24 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip
# Wed, 02 Feb 2022 13:41:27 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:41:28 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:41:30 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:41:35 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:41:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.2-beta
# Wed, 02 Feb 2022 13:41:39 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:41:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:43:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:43:45 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:43:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:44:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:44:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:44:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:45:03 GMT
USER 1001
# Wed, 02 Feb 2022 13:45:06 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:45:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:45:12 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29573a4b41f5943be6c257eef3d8ca9557fda050f890ae701b87f1cd5d8659be`  
		Last Modified: Wed, 02 Feb 2022 14:47:52 GMT  
		Size: 8.6 KB (8555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bd96fcb33b8970931372e1e180652ff0705e3408ec4dd3ff326f8faef69176`  
		Last Modified: Wed, 02 Feb 2022 14:47:49 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539fd520a237ed8a73b65529c8d68a07e510bc425ace62cd244df963d42be71f`  
		Last Modified: Wed, 02 Feb 2022 14:48:15 GMT  
		Size: 300.5 MB (300488310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4d66bee1bec041f7414cb9349eec04587cedc70762d2359978ee911d536add`  
		Last Modified: Wed, 02 Feb 2022 14:47:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea6276c379cedb58a402bd7fba6982665cade98291c0fd352fefb270e86d36`  
		Last Modified: Wed, 02 Feb 2022 14:47:49 GMT  
		Size: 10.1 KB (10073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2994e723049f878addf0342130dbbb27725370699de3d400fb520d3f6f5325`  
		Last Modified: Wed, 02 Feb 2022 14:47:52 GMT  
		Size: 12.2 MB (12206712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; s390x

```console
$ docker pull open-liberty@sha256:b732e3a50fa60d70f271034be80e430320eaf95559147728de8257c67e76d05b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.2 MB (408179013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb5fc89203fe3d7d90fb636880318b2e37aa713e2e01083e3ab83e2620f53c8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:52:51 GMT
ARG LIBERTY_VERSION=22.0.0.2-beta
# Wed, 02 Feb 2022 04:52:51 GMT
ARG LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8
# Wed, 02 Feb 2022 04:52:51 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:52:51 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip
# Wed, 02 Feb 2022 04:52:51 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:52:51 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:52:52 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:52:52 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:52:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.2-beta
# Wed, 02 Feb 2022 04:52:52 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:52:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:53:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:53:45 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:53:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:53:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:54:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.2-beta/openliberty-runtime-22.0.0.2-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=d5efb53c4f412eefed2c68b870d0fcd725fde6a8 LIBERTY_VERSION=22.0.0.2-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:54:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:54:10 GMT
USER 1001
# Wed, 02 Feb 2022 04:54:10 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:54:10 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:54:10 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e47e643d01b1cc932fa3ea4e9612b2390dfe5bf6a4702bc21faf23e154a263`  
		Last Modified: Wed, 02 Feb 2022 05:06:29 GMT  
		Size: 8.5 KB (8549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced0360f91f6ea78750bd023459718ea026824b4ee3ac4292b775d39c0e0bda5`  
		Last Modified: Wed, 02 Feb 2022 05:06:27 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a01dd0ab29ac39a537d923cce8b8b174cc59bef87bf8ed4aba89a800aae34b`  
		Last Modified: Wed, 02 Feb 2022 05:06:39 GMT  
		Size: 300.5 MB (300487905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dbf44953a912e831450944cbf8f2e168b92d75ec9d671f857ffc9a7dc26eb0`  
		Last Modified: Wed, 02 Feb 2022 05:06:27 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b291a8684e0b9989058eb07e1a1c1b3ca6babd1735046282d1f5441d1115327d`  
		Last Modified: Wed, 02 Feb 2022 05:06:27 GMT  
		Size: 10.0 KB (10037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1cecad4e579737dbd3ca6aaa820214c8713ff940e8919824ce2e65a9a90cb4`  
		Last Modified: Wed, 02 Feb 2022 05:06:29 GMT  
		Size: 13.8 MB (13840434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:0f169a11e9f2ece11364f95981929068c575c908fa4b78a4edaad5d796ea9c50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:d765a38c29f93b182c2ad64252826f928d1e2388014a4375936f2ac1e6fe806c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.1 MB (404055676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4363749360ffcb5d9356a2d92c680c8bef4c59cc5bd68de98c7048ddcaa3d219`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:16:04 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:04 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:16:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:16:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:16:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:16:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:17:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:17:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:17:14 GMT
USER 1001
# Tue, 01 Feb 2022 02:17:14 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:17:14 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:17:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0dd06f22af6d321debcc35fe49584e9508f3f8a9a34c9529a161d3b1d5859`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d871f90dc74ad1930ad07a28487c241564a95b4c2c807fa7498d7e6a00f071`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab0cd22ea6a2058ef644493e80d0144abf96f82cc9eb6268ff21383e96b39ad`  
		Last Modified: Tue, 01 Feb 2022 02:25:39 GMT  
		Size: 291.7 MB (291675718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb30f069fa13018d762521188faf3f255a2d9e2044dd45b46b39153623d89baa`  
		Last Modified: Tue, 01 Feb 2022 02:25:26 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c30df76bf4c02eaca50fee021d65c4d53ece95d36e1f22ebec0300d997b3102`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 10.1 KB (10052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22256b7cdc0b66dd775f30efcc4196b11b13ce4636d0b4bb4fcac17465b27d72`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 13.5 MB (13536116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:c37ba13362eed0a493c3e89984e50783f28f9e9e4a3a01bf3cab14119da1243c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.2 MB (408174413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a30cf262b777ee5a509f742afd88c46e29562fc9340f27cd185bb1de972d97d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:52:34 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 13:52:37 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:52:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 13:52:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:52:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:52:49 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:52:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:52:53 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:52:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:55:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:55:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:55:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:55:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:56:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:56:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:56:16 GMT
USER 1001
# Wed, 02 Feb 2022 13:56:17 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:56:20 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:56:22 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ec8b529c9dfc92f266863cb3cab0c9cabae82b6054a5ab6a102412d3d5c05`  
		Last Modified: Wed, 02 Feb 2022 14:48:57 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d314dc71e6bdf9b22e3000713842dfa6f7626239b3c3ffe91fce14937932fca`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0438eb8384253339c23764c856a2d4b4760d5cf877831869a445d300a612b`  
		Last Modified: Wed, 02 Feb 2022 14:49:20 GMT  
		Size: 291.7 MB (291676389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fdf6c1b7f149ace90882402b18a91bfb0f339f36ef947ba9e7a3d85d4f4a`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a1499353c85e51e33a6022fd6b6292d73d47bb334490c6444e464eb15f866f`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8db058827844fcef088df1ddeed8a6cebcf21d5add3cc4cb95cd3e16799756`  
		Last Modified: Wed, 02 Feb 2022 14:48:56 GMT  
		Size: 12.1 MB (12056712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:38ff00003cb886c8c096f1c2df08190807a59a10267c3796c49f471244ba0d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.9 MB (398879420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae86a30a90c24730c99c856a42bfecc96cea509d841bee1bd9b27b9da5e4622d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:55:58 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:55:58 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:58 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:55:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:55:58 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:55:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:56:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:56:25 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:56:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:56:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:56:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:56:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:56:46 GMT
USER 1001
# Wed, 02 Feb 2022 04:56:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:56:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:56:46 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3be9e00dbaa95dc5001e009e4a48f7bcb181012da6bcfbacd3faee29960d4e`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9128b48078d3a8f12b88808347a020a7df9f52091f1350c33a5c576d5bb665`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e5eb7eb37b3a087d8338dc2517841b9eaf4a37e546248bf50611c3fd162f76`  
		Last Modified: Wed, 02 Feb 2022 05:07:10 GMT  
		Size: 291.7 MB (291675971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ec240b69b0c5e711e0e971ace42fed0d4b1571aca08c322bb3829faf44c8b4`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bef308e4d233fd0433437d8949545adfdc3f22735b8a89def423c0b3204d08`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 10.0 KB (10043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc63c160bc902af47a99874236ba953f3cd6e49b192c16c0b1ab97881fd47f9b`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 10.8 MB (10825360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java11-openj9`

```console
$ docker pull open-liberty@sha256:0618eca4d60a4cf43ab63ad949f2c8270a27592c9d91059d218d85d8a27aca3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:56e6dbb0f19e2dc6a2a2bf15cd7824b4abaa6aa7327944cd265c33fb0e980f1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.3 MB (402259935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc588c675c48e3272cad11bb260bfb2edffde6824a252a33a0221258e49b8c6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Tue, 01 Feb 2022 02:17:26 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:17:27 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:17:27 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:17:27 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:17:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:17:27 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:17:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:17:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:17:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:17:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:17:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:18:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:18:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:18:16 GMT
USER 1001
# Tue, 01 Feb 2022 02:18:17 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:18:17 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:18:17 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502e7c64d459bd6cede5f1840b31534d4779e09fbcb65e2f9be1de2559f0a547`  
		Last Modified: Tue, 01 Feb 2022 02:25:53 GMT  
		Size: 8.6 KB (8550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a4ceef09c7c59993174e959a8c5e3abb92de69c67ae653181d4abbcc7b4319`  
		Last Modified: Tue, 01 Feb 2022 02:25:51 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2414052f962e781be1fc6a8b106e8c72454a9c648802ff5cbfa8cba5f8674179`  
		Last Modified: Tue, 01 Feb 2022 02:26:05 GMT  
		Size: 291.7 MB (291675754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ba754a35e035fe07a08616849f23364616b387b6c77dacba1e55e53e6d812`  
		Last Modified: Tue, 01 Feb 2022 02:25:51 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370d7762a1d46c1b36eeb7e9dc34daa38f957765fc1366e872fc3d1dc898ec5b`  
		Last Modified: Tue, 01 Feb 2022 02:25:51 GMT  
		Size: 10.0 KB (10042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d33103a128c06253c47add0ba6a3294ed03b45ffa95ca6de1eaafa1dd5aadf8`  
		Last Modified: Tue, 01 Feb 2022 02:25:54 GMT  
		Size: 13.9 MB (13850194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:b00bde9f06f57a1270f322ccd68a6da67f29d2352ac5698b02cd738b8f6098b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.1 MB (406084445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923cb9479651dadb1e85e2bcbff89dc395232cc5443d36fcd04f0ad24d9670d2`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:49:09 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:56:30 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 13:56:32 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:56:34 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 13:56:35 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:56:37 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:56:39 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:56:41 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:56:43 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:56:44 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:56:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 14:02:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 14:03:08 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 14:03:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 14:03:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 14:04:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 14:04:44 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 14:04:48 GMT
USER 1001
# Wed, 02 Feb 2022 14:04:51 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 14:04:56 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 14:04:59 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd519597fe72ce8b1344442be07458ad187acc1b64dbb8a8183487f749c3bbf1`  
		Last Modified: Wed, 02 Feb 2022 14:49:43 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4202f45c2725044fd3f9e269949a6abfc301d68711cde295b94430c51fd8d91`  
		Last Modified: Wed, 02 Feb 2022 14:49:40 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd99c0f2987d13cbaac5c80c3c8458227142ab88eed8a5302be3310cefa109`  
		Last Modified: Wed, 02 Feb 2022 14:50:10 GMT  
		Size: 291.7 MB (291676319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbaa8ff22cc19a669b732bc3738ce13926e7a7a8afb984f50bf842fe65a852a`  
		Last Modified: Wed, 02 Feb 2022 14:49:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb7bb68083573cc3090729eab966810568d852124913ca1fde3149f5fd7e8e`  
		Last Modified: Wed, 02 Feb 2022 14:49:40 GMT  
		Size: 10.1 KB (10067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347d59b924351befed80c43cc6ad75ce4c6ff319cec64482eb23663a83c9ec11`  
		Last Modified: Wed, 02 Feb 2022 14:49:42 GMT  
		Size: 12.2 MB (12222949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:ec184e4c286813121b2577b305751a63e2051fa172a626acb753a3d5960810e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.4 MB (399367610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427e39802d3664950186cc709ca9c13969ff56d94458609dd53e78f2824e050b`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:55:32 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:56:54 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:56:55 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:56:55 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:56:55 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:56:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:56:55 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:56:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:58:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:58:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:58:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:58:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:58:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:58:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:58:27 GMT
USER 1001
# Wed, 02 Feb 2022 04:58:28 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:58:28 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:58:28 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b28a68eb26051df97c041b172e6d74d5ae5492b9a4bcea81c1864a715684c4`  
		Last Modified: Wed, 02 Feb 2022 05:07:21 GMT  
		Size: 8.5 KB (8546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73815e61f4386b4fb2ac962fd030d492696944cb09fcdbdc4df77b330aa2af`  
		Last Modified: Wed, 02 Feb 2022 05:07:20 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30796d6efd8445365a3305a06c487082d82c3818a46b57cf03dee4c44c6a8718`  
		Last Modified: Wed, 02 Feb 2022 05:07:32 GMT  
		Size: 291.7 MB (291675973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d176335a99e00c1470f24b01881466ed7637c4d657bf693f3258836a4b91a43`  
		Last Modified: Wed, 02 Feb 2022 05:07:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1797525c5fbb7f0a412d0862ffddd68c605975b9e863a0499a246b71695ed2`  
		Last Modified: Wed, 02 Feb 2022 05:07:20 GMT  
		Size: 10.0 KB (10041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dacfbdebf94b1dc6f136bf8c17218209e5885b9c311a6687b300a40337e12bf`  
		Last Modified: Wed, 02 Feb 2022 05:07:21 GMT  
		Size: 13.8 MB (13840963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java8-openj9`

```console
$ docker pull open-liberty@sha256:0f169a11e9f2ece11364f95981929068c575c908fa4b78a4edaad5d796ea9c50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:d765a38c29f93b182c2ad64252826f928d1e2388014a4375936f2ac1e6fe806c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.1 MB (404055676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4363749360ffcb5d9356a2d92c680c8bef4c59cc5bd68de98c7048ddcaa3d219`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:16:04 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:04 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:16:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:16:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:16:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:16:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:17:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:17:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:17:14 GMT
USER 1001
# Tue, 01 Feb 2022 02:17:14 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:17:14 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:17:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0dd06f22af6d321debcc35fe49584e9508f3f8a9a34c9529a161d3b1d5859`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d871f90dc74ad1930ad07a28487c241564a95b4c2c807fa7498d7e6a00f071`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab0cd22ea6a2058ef644493e80d0144abf96f82cc9eb6268ff21383e96b39ad`  
		Last Modified: Tue, 01 Feb 2022 02:25:39 GMT  
		Size: 291.7 MB (291675718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb30f069fa13018d762521188faf3f255a2d9e2044dd45b46b39153623d89baa`  
		Last Modified: Tue, 01 Feb 2022 02:25:26 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c30df76bf4c02eaca50fee021d65c4d53ece95d36e1f22ebec0300d997b3102`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 10.1 KB (10052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22256b7cdc0b66dd775f30efcc4196b11b13ce4636d0b4bb4fcac17465b27d72`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 13.5 MB (13536116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:c37ba13362eed0a493c3e89984e50783f28f9e9e4a3a01bf3cab14119da1243c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.2 MB (408174413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a30cf262b777ee5a509f742afd88c46e29562fc9340f27cd185bb1de972d97d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:52:34 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 13:52:37 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:52:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 13:52:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:52:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:52:49 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:52:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:52:53 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:52:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:55:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:55:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:55:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:55:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:56:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:56:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:56:16 GMT
USER 1001
# Wed, 02 Feb 2022 13:56:17 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:56:20 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:56:22 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ec8b529c9dfc92f266863cb3cab0c9cabae82b6054a5ab6a102412d3d5c05`  
		Last Modified: Wed, 02 Feb 2022 14:48:57 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d314dc71e6bdf9b22e3000713842dfa6f7626239b3c3ffe91fce14937932fca`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0438eb8384253339c23764c856a2d4b4760d5cf877831869a445d300a612b`  
		Last Modified: Wed, 02 Feb 2022 14:49:20 GMT  
		Size: 291.7 MB (291676389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fdf6c1b7f149ace90882402b18a91bfb0f339f36ef947ba9e7a3d85d4f4a`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a1499353c85e51e33a6022fd6b6292d73d47bb334490c6444e464eb15f866f`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8db058827844fcef088df1ddeed8a6cebcf21d5add3cc4cb95cd3e16799756`  
		Last Modified: Wed, 02 Feb 2022 14:48:56 GMT  
		Size: 12.1 MB (12056712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:38ff00003cb886c8c096f1c2df08190807a59a10267c3796c49f471244ba0d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.9 MB (398879420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae86a30a90c24730c99c856a42bfecc96cea509d841bee1bd9b27b9da5e4622d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:55:58 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:55:58 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:58 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:55:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:55:58 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:55:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:56:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:56:25 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:56:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:56:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:56:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:56:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:56:46 GMT
USER 1001
# Wed, 02 Feb 2022 04:56:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:56:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:56:46 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3be9e00dbaa95dc5001e009e4a48f7bcb181012da6bcfbacd3faee29960d4e`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9128b48078d3a8f12b88808347a020a7df9f52091f1350c33a5c576d5bb665`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e5eb7eb37b3a087d8338dc2517841b9eaf4a37e546248bf50611c3fd162f76`  
		Last Modified: Wed, 02 Feb 2022 05:07:10 GMT  
		Size: 291.7 MB (291675971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ec240b69b0c5e711e0e971ace42fed0d4b1571aca08c322bb3829faf44c8b4`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bef308e4d233fd0433437d8949545adfdc3f22735b8a89def423c0b3204d08`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 10.0 KB (10043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc63c160bc902af47a99874236ba953f3cd6e49b192c16c0b1ab97881fd47f9b`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 10.8 MB (10825360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-slim`

```console
$ docker pull open-liberty@sha256:b02e7de7e19bb016efaf082af181c3ba3678b807ae993830899fd519a77c59e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim` - linux; amd64

```console
$ docker pull open-liberty@sha256:331e97c4e89399cfaa922e66788752932dd920d11c21476ba2874633e0a09525
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113096280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adbc584c36ae3c4eab850f94fcb0dd9ad46784ae4f0050f0bd5ed1dc0f21c80e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:15:22 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:22 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:15:22 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:15:22 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:15:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:15:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:15:28 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:15:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:15:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:15:37 GMT
USER 1001
# Tue, 01 Feb 2022 02:15:37 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:15:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:15:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdca4a06ca8bdadbdfced7e1e293379dfa19d8c6267d805bd23cceeb7b4f28a`  
		Last Modified: Tue, 01 Feb 2022 02:25:06 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915ee96ab3c294a6cebf8f011b1d6c832a87073596878d8bb438a243ec24fb28`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e881d56be87250c1d78d22954a8a10c6db9aa7fe53e830a923ff1ac9cd0a0a85`  
		Last Modified: Tue, 01 Feb 2022 02:25:05 GMT  
		Size: 11.8 MB (11814321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf9961f6b52f2af462e9ad187230136d1c92cc2e676edbcb3281d355f72f72`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f112feffa1f30cf33f0988bd507269849e1ad1e1ce9c700ae08d556e720707`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 9.2 KB (9211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e412099596dad8b30bb0704bb2812daf9535e73de582880fa415e84f8a2b748`  
		Last Modified: Tue, 01 Feb 2022 02:25:05 GMT  
		Size: 2.4 MB (2439725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:95dc78c596863727e7e53f9e3a869f4f3dce720385ae70cf58f54dfce85f69cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118667124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd88fd7312cb7cba7b1001eb57aefeb6b2e09bc1d4082d102066851702a66cb5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:45:31 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 13:45:35 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:45:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 13:45:41 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:45:43 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:45:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:45:48 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:45:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:45:51 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:45:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:48:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:48:19 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:48:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:48:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:48:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:48:53 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:48:56 GMT
USER 1001
# Wed, 02 Feb 2022 13:48:57 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:48:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:49:01 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b9604213edbe2684cacee5c5d17ff9922642da340455dacb9fb7079e5f5442`  
		Last Modified: Wed, 02 Feb 2022 14:48:28 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35fcc8a334d355228479a7b9f29038bbd05e7fa176b00289b25e900343d9fab`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ddb0cab9d3f827f351bfe1c1e251a7ba45a4b75542c906b5ea0ab2321577f`  
		Last Modified: Wed, 02 Feb 2022 14:48:27 GMT  
		Size: 11.8 MB (11815006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf24a37641ad7ae733bb4c1ef9f67a5e8044fa1720d665f71013d9be824ab5c2`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c472c2f1ff5cd1610a38158f47f53b6618efc7cc3625bd66e94e05eb46e9845`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 9.2 KB (9240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aff7a56991fd0349ecd9980c613d57a6c20786f91bdeab5a6fa73a4d0b1c5e5`  
		Last Modified: Wed, 02 Feb 2022 14:48:25 GMT  
		Size: 2.4 MB (2412396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim` - linux; s390x

```console
$ docker pull open-liberty@sha256:6a02f53d7133be6696647095385a6f0206abe3b60d70d4904e329fc1e5b70ce1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110433107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01a915d38097f490c316613b2d1f86e23ac1822790f90e9278d1bb4d808ac40c`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:54:25 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:54:25 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:54:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:54:26 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:54:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:55:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:55:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:55:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:55:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:55:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:55:25 GMT
USER 1001
# Wed, 02 Feb 2022 04:55:25 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:55:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:55:25 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae67e91b406ba6c368b5cf5e1d449b3d23ec4d15803d2c72d7c6a128d7103e63`  
		Last Modified: Wed, 02 Feb 2022 05:06:46 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2684cfa6bf38124a704e6111da0a41c4b3fa4fa2738734f8f3151263b86cc89a`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da325492888060446c03d0332f5cf21f4e89b29ef0d229ea913a10879418bcb9`  
		Last Modified: Wed, 02 Feb 2022 05:06:46 GMT  
		Size: 11.8 MB (11814528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95fac8ac0494f895f01fe281e4c8dddd12a382e8d4332723af592d36aaed758`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ed72f7e97cc70a57c36cd0124a7e7fa863a7fb62d8c94b3bcb35ae300d88be`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 9.2 KB (9219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c00e6613a88743d6bd75a56a43d670fdea29658113e6348ad3782760f818367`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 2.2 MB (2242073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-slim-java11-openj9`

```console
$ docker pull open-liberty@sha256:368eb70918ec75b0c7188eac8eda14ea184613e778dc2185818ee9bdfead8ebb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:5f930e67e211063a5947a13d25f8814b4820e0cc2a7d723b7d4186b1d8014c1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111003271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435d4b0d4a8948c126cc5f8c2f82142019407e21797ec221e4b10724ab88ac24`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:46:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:46:09 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:46:49 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:15:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Tue, 01 Feb 2022 02:15:41 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:15:41 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:15:41 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:41 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:15:41 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:15:42 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:15:42 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:15:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:15:47 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:15:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:15:57 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:15:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:15:57 GMT
USER 1001
# Tue, 01 Feb 2022 02:15:57 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:15:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:15:58 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f76e189bf5aa40f945426d7b5bd241778d681954e4d7b3393c8e46442b972e4`  
		Last Modified: Tue, 01 Feb 2022 01:55:36 GMT  
		Size: 47.7 MB (47658212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecdc661c2645b080ed6698be7a920e5790ae3d9dc9da34edbdcebcd2b2db13`  
		Last Modified: Tue, 01 Feb 2022 01:55:31 GMT  
		Size: 4.5 MB (4456772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ad96cb23fd36be631079e155934175b17d24fab63cdf253ef96d530e597af`  
		Last Modified: Tue, 01 Feb 2022 02:25:18 GMT  
		Size: 8.1 KB (8112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebc94632c966c3394394e1eee7b98294808a90fa5111425a2f12cd0faa09bf5`  
		Last Modified: Tue, 01 Feb 2022 02:25:16 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c807b8634aa793a3eb773f15c494e35eece09b87817ee6a454df02bbc2a32687`  
		Last Modified: Tue, 01 Feb 2022 02:25:17 GMT  
		Size: 11.8 MB (11814321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6014a014aeb2d7275c8be20d69db6735e8e2c31aaadb00cc72b7574d951673d`  
		Last Modified: Tue, 01 Feb 2022 02:25:16 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a069f334ed8c9cbda175ab76a832c4eadfd6d07543581b4e7c21a2d7deb6185`  
		Last Modified: Tue, 01 Feb 2022 02:25:17 GMT  
		Size: 9.2 KB (9222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8882a6d4d985523ebab8a95360e1dcdfd2f97e5ef3633376f79b5f32cdb12`  
		Last Modified: Tue, 01 Feb 2022 02:25:16 GMT  
		Size: 2.5 MB (2456554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:9d789995f5a4176331fb218d86c2710a3e401f904c0e96e136fc2b6af3700041
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116433217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb3e7377f72980e4b12a8234a3e958c425ce253fa7a65e96f7ef76d10913e36`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:48:18 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 06:50:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:50:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:51:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:49:09 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:49:12 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 13:49:14 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:49:15 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 13:49:19 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:49:20 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:49:24 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:49:26 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:49:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:49:32 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:49:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:51:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:51:24 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:51:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:51:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:52:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:52:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:52:11 GMT
USER 1001
# Wed, 02 Feb 2022 13:52:15 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:52:16 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:52:20 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc61c6b215f4fb7c75e6582ef6007365906c4e14cde00f0965b8779593d0c18e`  
		Last Modified: Wed, 02 Feb 2022 07:01:42 GMT  
		Size: 48.4 MB (48356080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b3efdb449fc2698509a19de1bfc1b98f4700a4daf3778eca7819346874810`  
		Last Modified: Wed, 02 Feb 2022 07:01:34 GMT  
		Size: 3.3 MB (3317348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c872852080f61b21851572b031d3eef74ac2eed627323c0be7936c9029e1b9b5`  
		Last Modified: Wed, 02 Feb 2022 14:48:45 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd8a421d5324e1d3cd3379bc54bcf2cd07fdd1b8acc576b5ccb2ae3d824e42e`  
		Last Modified: Wed, 02 Feb 2022 14:48:42 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b59ffab32c7a4660da62455898e020beb97ac6c59848b9898c4a3a0a5a9a84d`  
		Last Modified: Wed, 02 Feb 2022 14:48:43 GMT  
		Size: 11.8 MB (11814988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c721178cfe52334d7354db94a334c24322e6082478096d5599a66714331bf65`  
		Last Modified: Wed, 02 Feb 2022 14:48:42 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e43cd69d36c3f095cecf827cb691d95ff30003a50312860be68259e56b8954d`  
		Last Modified: Wed, 02 Feb 2022 14:48:42 GMT  
		Size: 9.2 KB (9235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4af65f391d30393f64b1fb0659065b4717f2bc51a50ab7ffb2ffb99274281f`  
		Last Modified: Wed, 02 Feb 2022 14:48:43 GMT  
		Size: 2.4 MB (2434644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:42b1100930cc8f72129d9f419f732692597f4d374dc665b89ed7509b76c3b64b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108136071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99dae7bcc64140db9458f25eacb72497b5477df1b9122b3cd89df1d12fb2ec17`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:30:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Wed, 02 Feb 2022 02:31:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:31:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:31:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:55:32 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:55:32 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:55:33 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:55:33 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:33 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:55:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:55:34 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:55:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:55:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:55:42 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:55:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:55:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:55:49 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:55:49 GMT
USER 1001
# Wed, 02 Feb 2022 04:55:49 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:55:49 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:55:49 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09d52708cad584b91766853829c0f7049699e2af2c9cafe7c13938e52baa8b`  
		Last Modified: Wed, 02 Feb 2022 02:37:39 GMT  
		Size: 46.7 MB (46692346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7329c8a16734bfb760ee4fd3751c0bbc084603d514980f3d1964a124899fb24`  
		Last Modified: Wed, 02 Feb 2022 02:37:33 GMT  
		Size: 4.3 MB (4279805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529b12ae434e8444f3f02fac8a9ea9bfa3b593462e008d2eaa1b53168d2ff808`  
		Last Modified: Wed, 02 Feb 2022 05:06:54 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e8f07cb58b2bafceaf238d7823cdf81f79d182ad8155b1a2c8220f2b73a26a`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36adbade8d4ef4a2f5441b06bc817a666fb690fb34a471740da6139d76f6bf20`  
		Last Modified: Wed, 02 Feb 2022 05:06:54 GMT  
		Size: 11.8 MB (11814539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9907e3b73349d5b48d31826024581694319df42403bcf4f2c74993e7157f0529`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f005f776114fec1122eef836d55dd09deb87c6fc367470bf77eb22255cc470ff`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 9.2 KB (9213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7f5aaed942ab6af3b8e2dd2b26439d8c5978259dc806572f3235c20e1bb8`  
		Last Modified: Wed, 02 Feb 2022 05:06:53 GMT  
		Size: 2.5 MB (2472444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:b02e7de7e19bb016efaf082af181c3ba3678b807ae993830899fd519a77c59e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:331e97c4e89399cfaa922e66788752932dd920d11c21476ba2874633e0a09525
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113096280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adbc584c36ae3c4eab850f94fcb0dd9ad46784ae4f0050f0bd5ed1dc0f21c80e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:15:21 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:15:22 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:22 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:15:22 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:15:22 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:15:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:15:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:15:28 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:15:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:15:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:15:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:15:37 GMT
USER 1001
# Tue, 01 Feb 2022 02:15:37 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:15:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:15:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdca4a06ca8bdadbdfced7e1e293379dfa19d8c6267d805bd23cceeb7b4f28a`  
		Last Modified: Tue, 01 Feb 2022 02:25:06 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915ee96ab3c294a6cebf8f011b1d6c832a87073596878d8bb438a243ec24fb28`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e881d56be87250c1d78d22954a8a10c6db9aa7fe53e830a923ff1ac9cd0a0a85`  
		Last Modified: Tue, 01 Feb 2022 02:25:05 GMT  
		Size: 11.8 MB (11814321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf9961f6b52f2af462e9ad187230136d1c92cc2e676edbcb3281d355f72f72`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f112feffa1f30cf33f0988bd507269849e1ad1e1ce9c700ae08d556e720707`  
		Last Modified: Tue, 01 Feb 2022 02:25:04 GMT  
		Size: 9.2 KB (9211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e412099596dad8b30bb0704bb2812daf9535e73de582880fa415e84f8a2b748`  
		Last Modified: Tue, 01 Feb 2022 02:25:05 GMT  
		Size: 2.4 MB (2439725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:95dc78c596863727e7e53f9e3a869f4f3dce720385ae70cf58f54dfce85f69cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118667124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd88fd7312cb7cba7b1001eb57aefeb6b2e09bc1d4082d102066851702a66cb5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:45:31 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 13:45:35 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:45:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 13:45:41 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:45:43 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:45:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:45:48 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:45:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:45:51 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:45:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:48:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:48:19 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:48:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:48:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:48:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:48:53 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:48:56 GMT
USER 1001
# Wed, 02 Feb 2022 13:48:57 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:48:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:49:01 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b9604213edbe2684cacee5c5d17ff9922642da340455dacb9fb7079e5f5442`  
		Last Modified: Wed, 02 Feb 2022 14:48:28 GMT  
		Size: 8.1 KB (8109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35fcc8a334d355228479a7b9f29038bbd05e7fa176b00289b25e900343d9fab`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ddb0cab9d3f827f351bfe1c1e251a7ba45a4b75542c906b5ea0ab2321577f`  
		Last Modified: Wed, 02 Feb 2022 14:48:27 GMT  
		Size: 11.8 MB (11815006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf24a37641ad7ae733bb4c1ef9f67a5e8044fa1720d665f71013d9be824ab5c2`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c472c2f1ff5cd1610a38158f47f53b6618efc7cc3625bd66e94e05eb46e9845`  
		Last Modified: Wed, 02 Feb 2022 14:48:24 GMT  
		Size: 9.2 KB (9240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aff7a56991fd0349ecd9980c613d57a6c20786f91bdeab5a6fa73a4d0b1c5e5`  
		Last Modified: Wed, 02 Feb 2022 14:48:25 GMT  
		Size: 2.4 MB (2412396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:6a02f53d7133be6696647095385a6f0206abe3b60d70d4904e329fc1e5b70ce1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110433107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01a915d38097f490c316613b2d1f86e23ac1822790f90e9278d1bb4d808ac40c`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:54:25 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:54:25 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:54:25 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:54:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:54:26 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:54:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:55:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:55:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:55:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:55:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.1/openliberty-kernel-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=21bc82aa555453d10971d0db2ebee483490e2f19 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:55:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:55:25 GMT
USER 1001
# Wed, 02 Feb 2022 04:55:25 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:55:25 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:55:25 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae67e91b406ba6c368b5cf5e1d449b3d23ec4d15803d2c72d7c6a128d7103e63`  
		Last Modified: Wed, 02 Feb 2022 05:06:46 GMT  
		Size: 8.1 KB (8111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2684cfa6bf38124a704e6111da0a41c4b3fa4fa2738734f8f3151263b86cc89a`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da325492888060446c03d0332f5cf21f4e89b29ef0d229ea913a10879418bcb9`  
		Last Modified: Wed, 02 Feb 2022 05:06:46 GMT  
		Size: 11.8 MB (11814528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95fac8ac0494f895f01fe281e4c8dddd12a382e8d4332723af592d36aaed758`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ed72f7e97cc70a57c36cd0124a7e7fa863a7fb62d8c94b3bcb35ae300d88be`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 9.2 KB (9219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c00e6613a88743d6bd75a56a43d670fdea29658113e6348ad3782760f818367`  
		Last Modified: Wed, 02 Feb 2022 05:06:45 GMT  
		Size: 2.2 MB (2242073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:0f169a11e9f2ece11364f95981929068c575c908fa4b78a4edaad5d796ea9c50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:d765a38c29f93b182c2ad64252826f928d1e2388014a4375936f2ac1e6fe806c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.1 MB (404055676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4363749360ffcb5d9356a2d92c680c8bef4c59cc5bd68de98c7048ddcaa3d219`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:41:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:49:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:40:40 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Tue, 01 Feb 2022 01:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:43:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:15:20 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:16:03 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Tue, 01 Feb 2022 02:16:04 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Tue, 01 Feb 2022 02:16:04 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:04 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:16:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Tue, 01 Feb 2022 02:16:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Tue, 01 Feb 2022 02:16:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Tue, 01 Feb 2022 02:16:41 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:16:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:16:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Tue, 01 Feb 2022 02:17:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Tue, 01 Feb 2022 02:17:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:17:14 GMT
USER 1001
# Tue, 01 Feb 2022 02:17:14 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:17:14 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:17:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e13f4c7fd2fb114074531c521dac0a966a3415bdd74da538677ecf096b757`  
		Last Modified: Fri, 07 Jan 2022 04:57:29 GMT  
		Size: 16.0 MB (16032427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a474728dc23a315fa700dbcb09bb2fc1ec4eb058693db3b868e811e4932a5`  
		Last Modified: Tue, 01 Feb 2022 01:54:11 GMT  
		Size: 50.0 MB (49952775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589c47c2c6025bd784de74f1734a228a03249979046e0d73625a41eba8066df`  
		Last Modified: Tue, 01 Feb 2022 01:54:04 GMT  
		Size: 4.3 MB (4272079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0dd06f22af6d321debcc35fe49584e9508f3f8a9a34c9529a161d3b1d5859`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d871f90dc74ad1930ad07a28487c241564a95b4c2c807fa7498d7e6a00f071`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab0cd22ea6a2058ef644493e80d0144abf96f82cc9eb6268ff21383e96b39ad`  
		Last Modified: Tue, 01 Feb 2022 02:25:39 GMT  
		Size: 291.7 MB (291675718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb30f069fa13018d762521188faf3f255a2d9e2044dd45b46b39153623d89baa`  
		Last Modified: Tue, 01 Feb 2022 02:25:26 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c30df76bf4c02eaca50fee021d65c4d53ece95d36e1f22ebec0300d997b3102`  
		Last Modified: Tue, 01 Feb 2022 02:25:25 GMT  
		Size: 10.1 KB (10052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22256b7cdc0b66dd775f30efcc4196b11b13ce4636d0b4bb4fcac17465b27d72`  
		Last Modified: Tue, 01 Feb 2022 02:25:27 GMT  
		Size: 13.5 MB (13536116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:c37ba13362eed0a493c3e89984e50783f28f9e9e4a3a01bf3cab14119da1243c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.2 MB (408174413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a30cf262b777ee5a509f742afd88c46e29562fc9340f27cd185bb1de972d97d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 06:45:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:45:24 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 06:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 06:47:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 06:47:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 06:47:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 13:45:29 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 13:52:34 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 13:52:37 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 13:52:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 13:52:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 13:52:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 13:52:45 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:52:49 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:52:51 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 13:52:53 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 13:52:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 13:55:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 13:55:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:55:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:55:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 13:56:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 13:56:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:56:16 GMT
USER 1001
# Wed, 02 Feb 2022 13:56:17 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:56:20 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:56:22 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14599df444bd4d5693103d52a497e59eae6815ba1988ceb343c30d5ee76d645`  
		Last Modified: Wed, 02 Feb 2022 07:00:07 GMT  
		Size: 17.2 MB (17206879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8da162146fc965a09c0c9cfc0fb5d7acec211da5a4e0a9258a17b79dcd3ea63`  
		Last Modified: Wed, 02 Feb 2022 07:00:44 GMT  
		Size: 50.4 MB (50445461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e713cec6e9261379537dbcf942d6205bcb9488c6dad73a38bf0cfe3970847a`  
		Last Modified: Wed, 02 Feb 2022 07:00:37 GMT  
		Size: 3.5 MB (3484103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ec8b529c9dfc92f266863cb3cab0c9cabae82b6054a5ab6a102412d3d5c05`  
		Last Modified: Wed, 02 Feb 2022 14:48:57 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d314dc71e6bdf9b22e3000713842dfa6f7626239b3c3ffe91fce14937932fca`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0438eb8384253339c23764c856a2d4b4760d5cf877831869a445d300a612b`  
		Last Modified: Wed, 02 Feb 2022 14:49:20 GMT  
		Size: 291.7 MB (291676389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fdf6c1b7f149ace90882402b18a91bfb0f339f36ef947ba9e7a3d85d4f4a`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a1499353c85e51e33a6022fd6b6292d73d47bb334490c6444e464eb15f866f`  
		Last Modified: Wed, 02 Feb 2022 14:48:54 GMT  
		Size: 10.1 KB (10064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8db058827844fcef088df1ddeed8a6cebcf21d5add3cc4cb95cd3e16799756`  
		Last Modified: Wed, 02 Feb 2022 14:48:56 GMT  
		Size: 12.1 MB (12056712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:38ff00003cb886c8c096f1c2df08190807a59a10267c3796c49f471244ba0d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.9 MB (398879420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae86a30a90c24730c99c856a42bfecc96cea509d841bee1bd9b27b9da5e4622d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:28:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:28:35 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Wed, 02 Feb 2022 02:29:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:29:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 02 Feb 2022 02:30:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 02 Feb 2022 04:54:24 GMT
ARG LIBERTY_VERSION=22.0.0.1
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip
# Wed, 02 Feb 2022 04:55:57 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 02 Feb 2022 04:55:58 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 02 Feb 2022 04:55:58 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:55:58 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 04:55:58 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.1
# Wed, 02 Feb 2022 04:55:58 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 02 Feb 2022 04:55:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 02 Feb 2022 04:56:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 02 Feb 2022 04:56:25 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 02 Feb 2022 04:56:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 04:56:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 02 Feb 2022 04:56:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl22.0.0.1920-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.1/openliberty-runtime-22.0.0.1.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9a5acc514c26ad91dadf9a21e5c61a090abf0dc9 LIBERTY_VERSION=22.0.0.1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 02 Feb 2022 04:56:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 04:56:46 GMT
USER 1001
# Wed, 02 Feb 2022 04:56:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 04:56:46 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 04:56:46 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066d7fe04dd83722853bf8aea5dff4791c6945ff1f246841815767944151d5a2`  
		Last Modified: Wed, 02 Feb 2022 02:36:46 GMT  
		Size: 15.7 MB (15739673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf536c7fab6c15b9963d713bc660a04e6bc5ee0f8ca9453c5d980a871f57cf31`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 49.2 MB (49184583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4124693144d33c1343b8c1d6549c80b297d937eaec88cf8c91d2a4a3ede61e97`  
		Last Modified: Wed, 02 Feb 2022 02:37:00 GMT  
		Size: 4.3 MB (4314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3be9e00dbaa95dc5001e009e4a48f7bcb181012da6bcfbacd3faee29960d4e`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9128b48078d3a8f12b88808347a020a7df9f52091f1350c33a5c576d5bb665`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e5eb7eb37b3a087d8338dc2517841b9eaf4a37e546248bf50611c3fd162f76`  
		Last Modified: Wed, 02 Feb 2022 05:07:10 GMT  
		Size: 291.7 MB (291675971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ec240b69b0c5e711e0e971ace42fed0d4b1571aca08c322bb3829faf44c8b4`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bef308e4d233fd0433437d8949545adfdc3f22735b8a89def423c0b3204d08`  
		Last Modified: Wed, 02 Feb 2022 05:06:59 GMT  
		Size: 10.0 KB (10043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc63c160bc902af47a99874236ba953f3cd6e49b192c16c0b1ab97881fd47f9b`  
		Last Modified: Wed, 02 Feb 2022 05:07:00 GMT  
		Size: 10.8 MB (10825360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
