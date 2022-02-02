<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `websphere-liberty`

-	[`websphere-liberty:21.0.0.12-full-java11-openj9`](#websphere-liberty210012-full-java11-openj9)
-	[`websphere-liberty:21.0.0.12-full-java8-ibmjava`](#websphere-liberty210012-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.12-kernel-java11-openj9`](#websphere-liberty210012-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.12-kernel-java8-ibmjava`](#websphere-liberty210012-kernel-java8-ibmjava)
-	[`websphere-liberty:21.0.0.9-full-java11-openj9`](#websphere-liberty21009-full-java11-openj9)
-	[`websphere-liberty:21.0.0.9-full-java8-ibmjava`](#websphere-liberty21009-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.9-kernel-java11-openj9`](#websphere-liberty21009-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.9-kernel-java8-ibmjava`](#websphere-liberty21009-kernel-java8-ibmjava)
-	[`websphere-liberty:22.0.0.1-full-java11-openj9`](#websphere-liberty22001-full-java11-openj9)
-	[`websphere-liberty:22.0.0.1-full-java8-ibmjava`](#websphere-liberty22001-full-java8-ibmjava)
-	[`websphere-liberty:22.0.0.1-kernel-java11-openj9`](#websphere-liberty22001-kernel-java11-openj9)
-	[`websphere-liberty:22.0.0.1-kernel-java8-ibmjava`](#websphere-liberty22001-kernel-java8-ibmjava)
-	[`websphere-liberty:full`](#websphere-libertyfull)
-	[`websphere-liberty:full-java11-openj9`](#websphere-libertyfull-java11-openj9)
-	[`websphere-liberty:kernel`](#websphere-libertykernel)
-	[`websphere-liberty:kernel-java11-openj9`](#websphere-libertykernel-java11-openj9)
-	[`websphere-liberty:latest`](#websphere-libertylatest)

## `websphere-liberty:21.0.0.12-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:52dd5597b3ffe023d18b2e0bd2ee11ced924b944d352db48864de66661f5539c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:657af8e9a23946f2a33e7253ea081c2edb78dfc5b7b63aff883ccca710dad563
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392575746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b134949590c1091fd7b7eb19158649873b8c328cdd7b4b11993dc03efd476548`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:14 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Tue, 01 Feb 2022 02:38:14 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Tue, 01 Feb 2022 02:38:15 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Tue, 01 Feb 2022 02:38:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:38:15 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Tue, 01 Feb 2022 02:38:15 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:38:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:38:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:38:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:38:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:38:25 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:38:26 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:38:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:38:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:38:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:38:35 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:38:35 GMT
USER 1001
# Tue, 01 Feb 2022 02:38:35 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:38:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:38:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:38:44 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:38:44 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:42:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:42:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:43:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:53edc8cc595f08a6f9ba4043fb3ca66fdbf01dbf3158cd9da12e79f58d8135cb`  
		Last Modified: Tue, 01 Feb 2022 02:49:00 GMT  
		Size: 14.3 MB (14286034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db727b29441d022b0d0b4ca3f9f1e35ae1a1d4b261e166513f11889affcb53d2`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bd9f95f4a8d4d16fb6d2ba1e2576660adc263a6a32df583fe6491a40c21081`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd9b0d7d198082ae34854e85a440a6d2452b7e706442f58727c8a5126685e8e`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13117f2d7f6313c0ea62519ee70d6c116aa4657d28d6d3ca9b93300b11d09bb3`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c68936ce12259761d2b6e1adca6d99b832c4e00f5c9ceddc64021ab50dba36`  
		Last Modified: Tue, 01 Feb 2022 02:48:57 GMT  
		Size: 2.5 MB (2508455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8422ba646f754cf914e478655fec69734f322540e82b998cb8098d8389e651eb`  
		Last Modified: Tue, 01 Feb 2022 02:49:20 GMT  
		Size: 264.6 MB (264634713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76115e1e1ced08f443df9b632a47aba7f7ebbda5cd9f2f47138d96eb5f75d467`  
		Last Modified: Tue, 01 Feb 2022 02:49:07 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6bbd2d16cbe1bc5b8c24eb3a20af145a6d069b0332f1989dc9a66bee1fe07`  
		Last Modified: Tue, 01 Feb 2022 02:49:09 GMT  
		Size: 14.4 MB (14410462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:1897c757d005f51aee8da6ee555840d60d901dbf7cc087e2e86ec37374faced0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396114136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34d89f401480d8985f6907f3d3591a285a96e6cf6ebdb128114d1c7c6f8a10d`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:54:00 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 12:54:01 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 12:54:02 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 12:54:05 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:54:07 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 12:54:09 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:54:10 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:58:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:58:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:58:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 12:59:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:59:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:59:08 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:59:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:59:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:59:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:59:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 12:59:35 GMT
USER 1001
# Wed, 02 Feb 2022 12:59:37 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:59:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:59:42 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 13:05:37 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:05:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 13:09:56 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 13:10:04 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 13:10:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:6d764e5856aeda2aa198a81f0a20bfc4b56b81be68d453a250ef24c288a2e533`  
		Last Modified: Wed, 02 Feb 2022 13:33:17 GMT  
		Size: 14.3 MB (14286672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186724339c086d9eda7af3960e7fa88d5dbe9b9aab1b5b1124a5276ecf832dfc`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303f749fe1b2d8965521298fb21ada9f590309b372cf6880fde859251ecee63`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1f9091177966d27487676e1cdbd06e729fcba7461d0ca2103f873cf4fb93e7`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46b1723808aa6fd654bbde92be9141449761a4b4dd773072ba84abb615baf1`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 10.7 KB (10663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c308b150e274e88d180166a70a89674b43e8d3fc6faa8bfd4855460c4a3521`  
		Last Modified: Wed, 02 Feb 2022 13:33:13 GMT  
		Size: 2.5 MB (2483685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392385e00a7941928496b95a572fdafebc8eff0050ae3924d6a5270eb5228bfa`  
		Last Modified: Wed, 02 Feb 2022 13:34:22 GMT  
		Size: 264.6 MB (264634653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f4e0665cb17fe14648b712fe0675bb47a78327d5d2c63c8721be338d2be3eb`  
		Last Modified: Wed, 02 Feb 2022 13:33:58 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7324fea7fbf7b81214ee6ff9755cebb1ef7aa4c095b83e590e88fb9f2999a70`  
		Last Modified: Wed, 02 Feb 2022 13:34:00 GMT  
		Size: 12.5 MB (12521860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:02420f2b1935ae9836508ef64108826d0dfac73178a642287fd4c3104917c6a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.6 MB (389589634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b8fad7d0a11df0a8d7814ed77c2a835979c6963b3cf39f6176b52b1c0e4ebe1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:21:17 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 05:21:17 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 05:21:17 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 05:21:17 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:21:18 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 05:21:18 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:21:18 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:21:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:21:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:21:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:21:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:21:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:21:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:21:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:21:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:21:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:21:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:21:36 GMT
USER 1001
# Wed, 02 Feb 2022 05:21:36 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:21:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:21:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:26:38 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:26:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:30:37 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:30:43 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:31:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:ebc3d0f22618ff7d12960afdb0bb0e516b4bed63fe764ebdee604d4155223478`  
		Last Modified: Wed, 02 Feb 2022 05:42:51 GMT  
		Size: 14.3 MB (14286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3099d5068ba1167247e10d64d0ea320e73236f26a25aabbdc3c854d3ed2baa57`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf51150d5dd7eb945723f412bf73c0a92353d63c47cea9f276a6e399b4efaf4`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d623712e5d3e2717abac06424c3363b30a03f43bfbafd5ab1d1888e67e878f1`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffe5b000132a5aa42920388b3629770a872df8ad6a6e0a4d94d461bc97a9b47`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe3c3604e43610f325792a106eb47fbe7d075d1a2c310f36b282d26a1efc45d`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 2.5 MB (2516957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b9aa6bc4d6e9d964fdf967cdd90d0c3b299377c03b6a429196f8c15db7a8d4`  
		Last Modified: Wed, 02 Feb 2022 05:43:24 GMT  
		Size: 264.6 MB (264635107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18b0bb6a2992e7c600e1a488a13ab96d6a1899f97a7426a4dfcdce32647c029`  
		Last Modified: Wed, 02 Feb 2022 05:43:13 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67c8c705f49800a8f9b6c21507c2699db16dabebd0426645294e0592a436ce8`  
		Last Modified: Wed, 02 Feb 2022 05:43:15 GMT  
		Size: 14.3 MB (14298516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:6cffe7b624aca0a96e75611aeb7793fb22ccc6b87d58d1a86cfa3db71f4dff89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:77f98951cf2b034cda64d90abfa699e0d8c6c3dd703aa1895a75f7766504e978
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.1 MB (459097141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee232ae5560eee5de20d5dbd17fa70b18f2081a70e330956f9ba0f1d75d56ced`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:21:48 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Fri, 07 Jan 2022 07:21:49 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Fri, 07 Jan 2022 07:21:49 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Fri, 07 Jan 2022 07:21:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:21:49 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Fri, 07 Jan 2022 07:21:49 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:21:50 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:22:02 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:22:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Fri, 07 Jan 2022 07:22:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:22:04 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:22:04 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:22:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:22:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:22:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:22:15 GMT
USER 1001
# Fri, 07 Jan 2022 07:22:15 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:22:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:22:16 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 07 Jan 2022 07:22:49 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:22:49 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 07 Jan 2022 07:26:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 07 Jan 2022 07:26:20 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 07 Jan 2022 07:26:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9438f70d1ec0ebbfd192b618dcb04d90dde46b1d82020fc2b471bb5d24658d0c`  
		Last Modified: Fri, 07 Jan 2022 07:40:08 GMT  
		Size: 14.2 MB (14187608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989cd92311688feaf6eb0b2666240028052f272be8cfe0976c5d83f96a5a7c9b`  
		Last Modified: Fri, 07 Jan 2022 07:40:05 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4407145761b640fb2995c090f0040de2c3e8d3135b6cc2e60db3f7b14c2489db`  
		Last Modified: Fri, 07 Jan 2022 07:40:04 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d64e67536bd53ec8035e3fe40f9fd6d9093ed63ef5f511cd61a53116e67e94`  
		Last Modified: Fri, 07 Jan 2022 07:40:04 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ac2083dc6ac5db7b9f3da5f665944cba08705d49a87afe6aa536b641fb47bb`  
		Last Modified: Fri, 07 Jan 2022 07:40:04 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bf26dcd0eee2488f65025dfd1c9d56ec2bebc476276ffc0dab4591ecfb7`  
		Last Modified: Fri, 07 Jan 2022 07:40:05 GMT  
		Size: 5.7 MB (5672502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1125618c37fe30a01f5f2b3e9485f3a51f527af21ea84199dbf3f974f84402b`  
		Last Modified: Fri, 07 Jan 2022 07:40:41 GMT  
		Size: 264.6 MB (264634716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a44f0dc5f87edba0c468439f055a248f89a953ab60e77523bfe88429638e6ef`  
		Last Modified: Fri, 07 Jan 2022 07:40:28 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b542381c72f37caadf829ee09257895e1da7563f920317b40c67cc8d6b0da51`  
		Last Modified: Fri, 07 Jan 2022 07:40:30 GMT  
		Size: 16.2 MB (16187989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:4514f5cfacd407e0020654dc07070c65c784763dd14ccb207634dee765b765e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.5 MB (459529955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032ca1a76a1117636aac13eea22f929fd71565eb69c0e97a1da94ace3fc502d2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:47:49 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 12:47:51 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 12:47:52 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 12:47:54 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:47:55 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 12:47:56 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:47:58 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:53:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:53:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:53:10 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 12:53:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:53:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:53:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:53:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:53:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:53:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:53:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:53:45 GMT
USER 1001
# Wed, 02 Feb 2022 12:53:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:53:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:53:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 12:59:56 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:59:58 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 13:04:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 13:04:23 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 13:05:20 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423ddd7370d8330d65c50ee07fb5171351afec5ebd9f9a1fa05a18f7f7fb024`  
		Last Modified: Wed, 02 Feb 2022 13:33:04 GMT  
		Size: 14.2 MB (14187565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b833b98cf2c4b6f082163929ff4253757cbd861e2710541b74019abfbe206c1a`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706962abf0035e8741c6bfd293960acbf8c54b2a672a50521d82a426b6412195`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f353728d6e512dc141c90a4f1845b953271f756dc9a0e22b9d05def0b438ab`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d434e9b85b432d75f420539395c48675c0cf57f0dd11afa06f80d521cb8b85`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5253f40c4557ecdb44d5c763405312665ea0d755a262d00af57c0f54d54946a4`  
		Last Modified: Wed, 02 Feb 2022 13:33:01 GMT  
		Size: 5.2 MB (5236099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f9c5e9cda8fc3c561c3e82057afb188483eaf84561f2c357cf8f906aa45666`  
		Last Modified: Wed, 02 Feb 2022 13:33:49 GMT  
		Size: 264.6 MB (264634883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2295d96bf361c21d639a904df08a21fc061e94294c19b0b214b895e387e2b4c`  
		Last Modified: Wed, 02 Feb 2022 13:33:25 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd1a7e3f3787f7a204e30b28ad99bfe5ae9275f4359bb12d4ebb35d59ac43cd`  
		Last Modified: Wed, 02 Feb 2022 13:33:29 GMT  
		Size: 13.7 MB (13673437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:b0c5bd09abc0ace64cf1159058dec18fa516e75b89faceec25d1e7745fe414f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.2 MB (454195189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8cb593f354e51fd7ef70b2ac28855f448d75525090681d2f7c1ff291718b904`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:20:49 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 05:20:49 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 05:20:49 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 05:20:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:20:50 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 05:20:50 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:20:50 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:21:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:21:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:21:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:21:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:21:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:21:02 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:21:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:21:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:21:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:21:10 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:21:10 GMT
USER 1001
# Wed, 02 Feb 2022 05:21:11 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:21:11 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:21:11 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:21:45 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:21:45 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:26:00 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:26:05 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:26:28 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa902a577eeeb7b8da2b38a80c16556aa25b473907be3c3a3b1cf5d0d4bf68`  
		Last Modified: Wed, 02 Feb 2022 05:42:44 GMT  
		Size: 14.2 MB (14187127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e1a54d736a7186929659809df2e6ea4b1bf3d414f78a286c31fac60c4eae48`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca933a76504ca86519f6e95f838b0bbfafbbbe78e35b379f6c93fd96335c7492`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2099aff1d7d293676bd61124a4b7e2d0a21867979fd683d49c3a9d5dd9cf2482`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f4bd2dc75e11c41e19aa59b798a9483ff603f8003cec71a00e578655d552d0`  
		Last Modified: Wed, 02 Feb 2022 05:42:41 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6a81a5adecd3d21c189ab8fcc0cfbe026b0a4c11350372c7f81526d9e699f`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 5.8 MB (5839486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92596fa070f1624527afc8885e5a3e0d83f1b498bbe1038159b4ab8620ac61a2`  
		Last Modified: Wed, 02 Feb 2022 05:43:08 GMT  
		Size: 264.6 MB (264635401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a8204a35cb9d5ca18a1282e44dd92a2cfe99c3950baf0b7c641f62f8161faa`  
		Last Modified: Wed, 02 Feb 2022 05:42:56 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c1b9f32464eff267bf3d4bdf5ed34d126468aeaf8c5e5bf8b9112233b89fcc`  
		Last Modified: Wed, 02 Feb 2022 05:42:58 GMT  
		Size: 15.7 MB (15732443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:19d0f1f5b34167ed76a6ce25fc8d90e81bcfdd8c2773b03a2c81464a538ec93c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:4b3d6c9d2bcf0577e38b6f913fce2ffb10ec192fa1f4ec9ce88327834ba13c7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113529624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89545c42caf8972290adf69adf817ffb74cd96d037720d7e33fc8477647b0291`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:14 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Tue, 01 Feb 2022 02:38:14 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Tue, 01 Feb 2022 02:38:15 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Tue, 01 Feb 2022 02:38:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:38:15 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Tue, 01 Feb 2022 02:38:15 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:38:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:38:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:38:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:38:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:38:25 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:38:26 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:38:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:38:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:38:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:38:35 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:38:35 GMT
USER 1001
# Tue, 01 Feb 2022 02:38:35 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:38:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:38:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:53edc8cc595f08a6f9ba4043fb3ca66fdbf01dbf3158cd9da12e79f58d8135cb`  
		Last Modified: Tue, 01 Feb 2022 02:49:00 GMT  
		Size: 14.3 MB (14286034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db727b29441d022b0d0b4ca3f9f1e35ae1a1d4b261e166513f11889affcb53d2`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bd9f95f4a8d4d16fb6d2ba1e2576660adc263a6a32df583fe6491a40c21081`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd9b0d7d198082ae34854e85a440a6d2452b7e706442f58727c8a5126685e8e`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13117f2d7f6313c0ea62519ee70d6c116aa4657d28d6d3ca9b93300b11d09bb3`  
		Last Modified: Tue, 01 Feb 2022 02:48:56 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c68936ce12259761d2b6e1adca6d99b832c4e00f5c9ceddc64021ab50dba36`  
		Last Modified: Tue, 01 Feb 2022 02:48:57 GMT  
		Size: 2.5 MB (2508455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:d253c3743b3e44ecbbe4615fb3b82b9eae075a547426a36b9a8f654cc8baa94c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118956677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ca3f68f70d7688519370b657f08be237ff81f2c0aef81614de3bc24271c0bce`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:54:00 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 12:54:01 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 12:54:02 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 12:54:05 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:54:07 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 12:54:09 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:54:10 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:58:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:58:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:58:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 12:59:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:59:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:59:08 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:59:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:59:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:59:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:59:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 12:59:35 GMT
USER 1001
# Wed, 02 Feb 2022 12:59:37 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:59:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:59:42 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:6d764e5856aeda2aa198a81f0a20bfc4b56b81be68d453a250ef24c288a2e533`  
		Last Modified: Wed, 02 Feb 2022 13:33:17 GMT  
		Size: 14.3 MB (14286672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186724339c086d9eda7af3960e7fa88d5dbe9b9aab1b5b1124a5276ecf832dfc`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303f749fe1b2d8965521298fb21ada9f590309b372cf6880fde859251ecee63`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1f9091177966d27487676e1cdbd06e729fcba7461d0ca2103f873cf4fb93e7`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46b1723808aa6fd654bbde92be9141449761a4b4dd773072ba84abb615baf1`  
		Last Modified: Wed, 02 Feb 2022 13:33:12 GMT  
		Size: 10.7 KB (10663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c308b150e274e88d180166a70a89674b43e8d3fc6faa8bfd4855460c4a3521`  
		Last Modified: Wed, 02 Feb 2022 13:33:13 GMT  
		Size: 2.5 MB (2483685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1487057a62db776f1e0580b5c8c315f3230253a89adf08e5e0f55ffdecc00b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110655063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4cad74a22d6e7bb5ef829415d1966ff7ffa103ba7951c83e7cfe5831393de70`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:21:17 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 05:21:17 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 05:21:17 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 05:21:17 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:21:18 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 05:21:18 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:21:18 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:21:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:21:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:21:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:21:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:21:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:21:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:21:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:21:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:21:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:21:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:21:36 GMT
USER 1001
# Wed, 02 Feb 2022 05:21:36 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:21:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:21:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:ebc3d0f22618ff7d12960afdb0bb0e516b4bed63fe764ebdee604d4155223478`  
		Last Modified: Wed, 02 Feb 2022 05:42:51 GMT  
		Size: 14.3 MB (14286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3099d5068ba1167247e10d64d0ea320e73236f26a25aabbdc3c854d3ed2baa57`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf51150d5dd7eb945723f412bf73c0a92353d63c47cea9f276a6e399b4efaf4`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d623712e5d3e2717abac06424c3363b30a03f43bfbafd5ab1d1888e67e878f1`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffe5b000132a5aa42920388b3629770a872df8ad6a6e0a4d94d461bc97a9b47`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe3c3604e43610f325792a106eb47fbe7d075d1a2c310f36b282d26a1efc45d`  
		Last Modified: Wed, 02 Feb 2022 05:42:49 GMT  
		Size: 2.5 MB (2516957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:64081fd24da4100a4ffea344ba18d071a16753b2e5d7026338538e64a66f4a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:09d89aa832a46d2a24a1f1544c06c73f307dc4e3c8e40fe4c7d8b97eb5b5e7fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178273490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318a803b271632a1dc557fe4dd7a06f19957bf79f0ecc96a86296020f7c8495e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:21:48 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Fri, 07 Jan 2022 07:21:49 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Fri, 07 Jan 2022 07:21:49 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Fri, 07 Jan 2022 07:21:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:21:49 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Fri, 07 Jan 2022 07:21:49 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:21:50 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:22:02 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:22:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Fri, 07 Jan 2022 07:22:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:22:04 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:22:04 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:22:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:22:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:22:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:22:15 GMT
USER 1001
# Fri, 07 Jan 2022 07:22:15 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:22:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:22:16 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9438f70d1ec0ebbfd192b618dcb04d90dde46b1d82020fc2b471bb5d24658d0c`  
		Last Modified: Fri, 07 Jan 2022 07:40:08 GMT  
		Size: 14.2 MB (14187608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989cd92311688feaf6eb0b2666240028052f272be8cfe0976c5d83f96a5a7c9b`  
		Last Modified: Fri, 07 Jan 2022 07:40:05 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4407145761b640fb2995c090f0040de2c3e8d3135b6cc2e60db3f7b14c2489db`  
		Last Modified: Fri, 07 Jan 2022 07:40:04 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d64e67536bd53ec8035e3fe40f9fd6d9093ed63ef5f511cd61a53116e67e94`  
		Last Modified: Fri, 07 Jan 2022 07:40:04 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ac2083dc6ac5db7b9f3da5f665944cba08705d49a87afe6aa536b641fb47bb`  
		Last Modified: Fri, 07 Jan 2022 07:40:04 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bf26dcd0eee2488f65025dfd1c9d56ec2bebc476276ffc0dab4591ecfb7`  
		Last Modified: Fri, 07 Jan 2022 07:40:05 GMT  
		Size: 5.7 MB (5672502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c1f9bb7d496ddde54870998fb7569036ff8b018d2f135082b419fc94b4e69a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.2 MB (181220688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152e1934d6f0f978f36f6b20598a5c03c64cbcd361589836859f186b3d494bb6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:47:49 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 12:47:51 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 12:47:52 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 12:47:54 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:47:55 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 12:47:56 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:47:58 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:53:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:53:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:53:10 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 12:53:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:53:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:53:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:53:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:53:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:53:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:53:43 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:53:45 GMT
USER 1001
# Wed, 02 Feb 2022 12:53:46 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:53:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:53:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423ddd7370d8330d65c50ee07fb5171351afec5ebd9f9a1fa05a18f7f7fb024`  
		Last Modified: Wed, 02 Feb 2022 13:33:04 GMT  
		Size: 14.2 MB (14187565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b833b98cf2c4b6f082163929ff4253757cbd861e2710541b74019abfbe206c1a`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706962abf0035e8741c6bfd293960acbf8c54b2a672a50521d82a426b6412195`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f353728d6e512dc141c90a4f1845b953271f756dc9a0e22b9d05def0b438ab`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d434e9b85b432d75f420539395c48675c0cf57f0dd11afa06f80d521cb8b85`  
		Last Modified: Wed, 02 Feb 2022 13:33:00 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5253f40c4557ecdb44d5c763405312665ea0d755a262d00af57c0f54d54946a4`  
		Last Modified: Wed, 02 Feb 2022 13:33:01 GMT  
		Size: 5.2 MB (5236099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:39d90113e067a2e816b48707ce333bb6ae2bb63898c3ea9dd28ae633382c3fde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.8 MB (173826399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4b317e69dee98c375eb48ff1e323b018d23a8bc43f721471da2e4c8cd868c9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:20:49 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 02 Feb 2022 05:20:49 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 02 Feb 2022 05:20:49 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 02 Feb 2022 05:20:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:20:50 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 02 Feb 2022 05:20:50 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:20:50 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:21:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:21:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:21:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Wed, 02 Feb 2022 05:21:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:21:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:21:02 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:21:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:21:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:21:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:21:10 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:21:10 GMT
USER 1001
# Wed, 02 Feb 2022 05:21:11 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:21:11 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:21:11 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa902a577eeeb7b8da2b38a80c16556aa25b473907be3c3a3b1cf5d0d4bf68`  
		Last Modified: Wed, 02 Feb 2022 05:42:44 GMT  
		Size: 14.2 MB (14187127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e1a54d736a7186929659809df2e6ea4b1bf3d414f78a286c31fac60c4eae48`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca933a76504ca86519f6e95f838b0bbfafbbbe78e35b379f6c93fd96335c7492`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2099aff1d7d293676bd61124a4b7e2d0a21867979fd683d49c3a9d5dd9cf2482`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f4bd2dc75e11c41e19aa59b798a9483ff603f8003cec71a00e578655d552d0`  
		Last Modified: Wed, 02 Feb 2022 05:42:41 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6a81a5adecd3d21c189ab8fcc0cfbe026b0a4c11350372c7f81526d9e699f`  
		Last Modified: Wed, 02 Feb 2022 05:42:42 GMT  
		Size: 5.8 MB (5839486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:97c4879280c00355bd8c930d1b1ba58b6910582324e51deeeeec4bda9a287713
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:67abbd202652c4b2df837bfe30ce0aa5cf97e7e2fbe5ddb2cbdc93c2afd51019
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (337011232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f482fb6b3a6c4cf5ffdf51f989d27620baa5625adbb9d9513156bf16386f4d`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:43:38 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 01 Feb 2022 02:43:38 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 01 Feb 2022 02:43:38 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 01 Feb 2022 02:43:39 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:43:39 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 01 Feb 2022 02:43:39 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:43:39 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:43:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:43:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:43:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 01 Feb 2022 02:43:49 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:43:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:43:50 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:43:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:43:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:43:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:43:59 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:43:59 GMT
USER 1001
# Tue, 01 Feb 2022 02:43:59 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:44:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:44:00 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:44:07 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:44:08 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:47:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:47:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:47:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:5967cc496b336b77788f8b96281e5121514cb12466e89ea1d90acc1b798fdb70`  
		Last Modified: Tue, 01 Feb 2022 02:49:32 GMT  
		Size: 14.2 MB (14154091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2146eddc57ad80094c99c027c82cb6ce1c43b9fb6b9e81291a6bff43df4fe763`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eaf55903fed7410878973b2c4ee38f79347f84fc37d132d0bfc0724b2ae710`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81dea0b66b77f1e606e24806edade85e0b555427056ddaeda302ca66f3deb0c`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b73e4ba5b3ddee35f19711dd363fe9470bf6c82236b52dee927e6614c80f7`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf34ff5ae175fc4b54c40b4aaf5887dbc3f9075fe2e8d17685c016d7a9bc08d`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 2.5 MB (2496458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e7b7ce49249e91530e7605df3e45f49c386c3397d1204101cd44dfb0bdff7`  
		Last Modified: Tue, 01 Feb 2022 02:49:50 GMT  
		Size: 209.2 MB (209236712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf68045a386086abf2a682ea7977985cc1e97256b196302c7545e5c5b6e9c6b`  
		Last Modified: Tue, 01 Feb 2022 02:49:39 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb3b8128f486ee593337edea22f2647eb64d4cc7ee9db72f57c2f4eaa68bbb`  
		Last Modified: Tue, 01 Feb 2022 02:49:42 GMT  
		Size: 14.4 MB (14387885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:0e883e40b2754e71487fd9e1a5753d0ab8a59ace46e5bb7e29ddf8001aad5cc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.3 MB (341347134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e31840c88a874fedf48ce42d185f3fec8a90e16da81057c39febf780d208fd5a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:14:30 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 13:14:32 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 13:14:35 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 13:14:39 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 13:14:42 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 13:14:44 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 13:14:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 13:17:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 13:17:28 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 13:17:32 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 13:17:36 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:17:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:17:47 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 13:17:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 13:17:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 13:18:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 13:18:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:18:20 GMT
USER 1001
# Wed, 02 Feb 2022 13:18:22 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:18:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:18:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 13:24:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:24:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 13:27:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 13:28:06 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 13:29:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:f07957a1221172c6788544c1d5be2c025db76a8192189c7e9816319ee45224d5`  
		Last Modified: Wed, 02 Feb 2022 13:34:50 GMT  
		Size: 14.2 MB (14154738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504594bd259b50a0a43a4929a9bd06b5135bc312c12ef736c9e468376bccf17`  
		Last Modified: Wed, 02 Feb 2022 13:34:44 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0a91ef55f0eb556d7f1dbc2d5abec025223c934b73d05998afa3f130167b25`  
		Last Modified: Wed, 02 Feb 2022 13:34:44 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa0922505eedd0e6a53a1a82d98f07d8e85d431ec2a2c3bd38a54668959fee2`  
		Last Modified: Wed, 02 Feb 2022 13:34:44 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862f3b11ae60d55d8da42b76c4c95d262accaef2c36bd8954da769f89f75d8a0`  
		Last Modified: Wed, 02 Feb 2022 13:34:45 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a06a09bb6f8a75e2b2a3fd31488c92810fad3792a00260b6ed4d4cf7c459c3`  
		Last Modified: Wed, 02 Feb 2022 13:34:45 GMT  
		Size: 2.5 MB (2459343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec98d8276de9031abed2f7dc6c7c6a8eadb0efae2d6ce54eff7d0e1cacaf3b22`  
		Last Modified: Wed, 02 Feb 2022 13:35:46 GMT  
		Size: 209.2 MB (209237082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeac0a7b5c85c84e77c4d349065f565f49dcce5d7f69367a95f5cb7ad2e3e11`  
		Last Modified: Wed, 02 Feb 2022 13:35:27 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26a2ba780fae1b1f8d443390d8f3b2dde133cbf781395d13b3c19be6d8d251d`  
		Last Modified: Wed, 02 Feb 2022 13:35:38 GMT  
		Size: 13.3 MB (13308695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:82f4beca3b806c3fdf01ac2928538bf8c611e5df4333683d3dcc2d4f4cdb2b9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334027265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a071d17aac24753e6bc5dfd9c60d65364a2caf74e0dac225edae6046d217762`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:31:48 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 05:31:48 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 05:31:48 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 05:31:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:31:48 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 05:31:49 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:31:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:31:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:32:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:32:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 05:32:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:32:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:32:01 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:32:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:32:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:32:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:32:08 GMT
USER 1001
# Wed, 02 Feb 2022 05:32:08 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:32:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:32:08 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:36:23 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:36:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:40:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:40:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:40:54 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:87898b3e11118d4555b22087ce18be3803af6a75379a4b35578d4254b6cb9796`  
		Last Modified: Wed, 02 Feb 2022 05:43:44 GMT  
		Size: 14.2 MB (14154300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e22c64bffc29b0c1f05ae6f680e70146130787d93915ccc3edecf2eea97b89`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae9936029879b0e5434e73148772ebcaf1d2dcdabd2d6487d134ed5e49f8eb8`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a613c6e9755c8568d36ae136a708f950c7c401e9181b802ad44fbb0f5673be`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d2c325811afdd268701b01df66e369940b62defd95f0ad7286cd5780bfd788`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 10.7 KB (10650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6fdf247b898594907c5bbdaa8fdd6c479f098c66aeeb8901b50d64c02bcc7`  
		Last Modified: Wed, 02 Feb 2022 05:43:42 GMT  
		Size: 2.5 MB (2508304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff027b6c0f434162bf09af85843c90085c354f171152915488a3a94342afdb3`  
		Last Modified: Wed, 02 Feb 2022 05:44:14 GMT  
		Size: 209.2 MB (209237739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8f3e523f3ee7c5ea0695d2958f7062b4b0b083212555a412a22f0712eea9b1`  
		Last Modified: Wed, 02 Feb 2022 05:44:05 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f644ec87f0d4ff7cd19feaeaaf5f31018fc28b121f50c5ae1cd5f7c3c40f964`  
		Last Modified: Wed, 02 Feb 2022 05:44:07 GMT  
		Size: 14.3 MB (14274143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:f759bba87cf51735d2894880b612dcc05c7ef9b41e493dfef36ff8ab26b01245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f06a0a8d03fc8809d26b39a691b83898f90b9ef1b32ccf4fb9cf527c5262be76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.4 MB (403357069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df0f50f297b7dcfe9f19b8d1b76a2e1d18fed1f3ac689ae4d2fd6a5766879a4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:31:42 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 07 Jan 2022 07:31:42 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 07 Jan 2022 07:31:42 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Fri, 07 Jan 2022 07:31:42 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:31:43 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Fri, 07 Jan 2022 07:31:43 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:31:43 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:31:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:31:53 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:31:53 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Fri, 07 Jan 2022 07:31:53 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:31:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:31:54 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:31:55 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:31:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:32:06 GMT
USER 1001
# Fri, 07 Jan 2022 07:32:06 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 07 Jan 2022 07:32:33 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:32:33 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 07 Jan 2022 07:35:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 07 Jan 2022 07:35:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 07 Jan 2022 07:36:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43504885995bd15c4af92a25a6359972b28b014371961dd90f79d1688adc18c`  
		Last Modified: Fri, 07 Jan 2022 07:41:28 GMT  
		Size: 14.1 MB (14056166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f069e2f59a77bfcbc1d5d2f8ae152ee5965c0f63d3d579e3ea2377c612da8dd5`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164b4defa73bd9deb729b95d6e68d37f1a3c292ae7c6ee6abae9dc9ce5f489e9`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6400ed0a0c0230917df6449d849dcde3a76292f48556ce6f276e0a0cca92723`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cc8fdcb84164f33db1d71b543f85b34719d9fcd4c0575b30f8fc22502727e8`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbd640931cdaa374c7241da9b00014a7740a80fc7a15facc8231df8a65917ac`  
		Last Modified: Fri, 07 Jan 2022 07:41:25 GMT  
		Size: 5.6 MB (5642065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2e57cc2a92ff76265e791d278e21d492a8059e38768371faf9e99e578e8a02`  
		Last Modified: Fri, 07 Jan 2022 07:41:56 GMT  
		Size: 209.2 MB (209236160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e31a283871ee7e3981a6ca4ab261cc0bdb9eaebc21b5ef4003a9dabd72cb77`  
		Last Modified: Fri, 07 Jan 2022 07:41:45 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6670c7b21e6a5d0db17aa217acf17b2e1b99a279998b2f1a5428a141a678a20b`  
		Last Modified: Fri, 07 Jan 2022 07:41:48 GMT  
		Size: 16.0 MB (16008376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:7ee920aeaa8aa4294bb11290587a82ed9125b7dbe944d31ee3d2bec2fdc46170
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.0 MB (404016968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5cf3d1cb4103c88cee8b283d3f0c04976e33fcc12684c283b7f0f60f4f682c6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:11:04 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 13:11:07 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 13:11:09 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 13:11:13 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 13:11:16 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 13:11:19 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 13:11:21 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 13:13:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 13:13:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 13:13:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 13:13:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:13:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:13:35 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 13:13:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 13:13:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 13:14:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 13:14:10 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 13:14:13 GMT
USER 1001
# Wed, 02 Feb 2022 13:14:15 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:14:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:14:18 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 13:18:40 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 13:18:42 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 13:22:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 13:22:58 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 13:24:00 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0008763388a9b63fabf4b13a6fec7a09a446d3282608474c642537c4904eaba5`  
		Last Modified: Wed, 02 Feb 2022 13:34:36 GMT  
		Size: 14.1 MB (14056148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feefa873c251180b540857621a8f0d44afe142654c3acbf2009e63a060fadf68`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39d715958173ac01bf793eef34a43223c968ee44f382c60af538e0dec45b5f3`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bea67f0ce83d7df3600b994d95ee04b0d319290d4889edc8e17cc0b6df55f8`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cdf9e22417e1ed70bfc90c84696bf0deedb986535f38c1dc83dd25c47e213b`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 10.7 KB (10661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cad774cff61a16f94c5f1737cc74eb758bc020d72345542762618a29cf8bdf7`  
		Last Modified: Wed, 02 Feb 2022 13:34:32 GMT  
		Size: 5.3 MB (5264168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983d9777ab97b8a43d3bc4669c730df71e4464ba2fd5b960deb1ecfff8c58121`  
		Last Modified: Wed, 02 Feb 2022 13:35:18 GMT  
		Size: 209.2 MB (209237472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7468aa4b33798612a4b4cc066fc5e513ebdb45433c6b9bc184fe3e4a4f61094`  
		Last Modified: Wed, 02 Feb 2022 13:34:59 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9552cadbb9fe27e8d52e08e50b2394afa0b5ab18eebedf24bc1c9995ae6517`  
		Last Modified: Wed, 02 Feb 2022 13:35:01 GMT  
		Size: 13.7 MB (13661197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0f6d273d1d76901101b120c735a5807e8a1a62b5acb5ef6ee70fefafdb7d6d3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.6 MB (398620688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d9499ee86e988b54cfd12614a91512d42900a1728f732ff35b4c9b59ba3b64`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:31:16 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 05:31:16 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 05:31:16 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 05:31:16 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:31:17 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 05:31:17 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:31:17 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:31:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:31:30 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:31:30 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 05:31:30 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:31:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:31:31 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:31:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:31:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:31:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:31:39 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:31:39 GMT
USER 1001
# Wed, 02 Feb 2022 05:31:39 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:31:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:31:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:32:16 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:32:16 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:35:36 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:35:41 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:36:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85402617352148106bf0a09a99cb07af7ffa2e47cafeb72b21e8526352180ec9`  
		Last Modified: Wed, 02 Feb 2022 05:43:37 GMT  
		Size: 14.1 MB (14055651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2cb196bf0e4bd26f0cd142b60a22b21b3aa9b89ef35dccfac1e171be77a687`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca286209f84c9c4eddb8358a213aca4ba7c55c9f33ebe205b5edd6dbe6122fb`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91066126bb9ae5d636277fe1a07f98dced5477bcec7aa9225907ee424dedb9d`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e37f2f3d254b346894c67e6524cbd8ac6d83ff75deb3c24d7779a49b5017f9`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f9af41e41b78737610210688142a4747597f12eb7fd06c3dc8ff88b5aad40a`  
		Last Modified: Wed, 02 Feb 2022 05:43:35 GMT  
		Size: 5.8 MB (5759525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c28af8912d2d5ab12f68b98feceeb8482eda56fcb938d2c3df524f2eb59fff5`  
		Last Modified: Wed, 02 Feb 2022 05:44:00 GMT  
		Size: 209.2 MB (209238040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30e511fac48f29746118d6f41c9ae336a8efa4b3b934e9b5c0a3ec8fe31219`  
		Last Modified: Wed, 02 Feb 2022 05:43:51 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82abd981e58128c66faccee8e2f04444c4828f5c7585be98f6b8513d7a15ac`  
		Last Modified: Wed, 02 Feb 2022 05:43:53 GMT  
		Size: 15.8 MB (15766737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:c09def988414e936a42458cbf1091156029a20ea229d685684275bed4ea59655
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:70da77713e14dbe875a2ad25090d8b210f275c05dd72dc4ae1ed2a7ad8906e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113385691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad31ad74e358177d2e6d76ab23bfbca5080b721ad07ad254ef7e4070816a9d5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:43:38 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 01 Feb 2022 02:43:38 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 01 Feb 2022 02:43:38 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 01 Feb 2022 02:43:39 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:43:39 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 01 Feb 2022 02:43:39 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:43:39 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:43:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:43:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:43:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 01 Feb 2022 02:43:49 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:43:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:43:50 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:43:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:43:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:43:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:43:59 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:43:59 GMT
USER 1001
# Tue, 01 Feb 2022 02:43:59 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:44:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:44:00 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:5967cc496b336b77788f8b96281e5121514cb12466e89ea1d90acc1b798fdb70`  
		Last Modified: Tue, 01 Feb 2022 02:49:32 GMT  
		Size: 14.2 MB (14154091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2146eddc57ad80094c99c027c82cb6ce1c43b9fb6b9e81291a6bff43df4fe763`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eaf55903fed7410878973b2c4ee38f79347f84fc37d132d0bfc0724b2ae710`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81dea0b66b77f1e606e24806edade85e0b555427056ddaeda302ca66f3deb0c`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b73e4ba5b3ddee35f19711dd363fe9470bf6c82236b52dee927e6614c80f7`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf34ff5ae175fc4b54c40b4aaf5887dbc3f9075fe2e8d17685c016d7a9bc08d`  
		Last Modified: Tue, 01 Feb 2022 02:49:29 GMT  
		Size: 2.5 MB (2496458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:2862bc4fed151e2795022b421032babc9498f10741c35793b8c534e3495ffdc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118800410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2be86117f2538acefdd0c3a5c2aa999b9444b56e96fe5544e86d2e9a23dfc1d`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:14:30 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 13:14:32 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 13:14:35 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 13:14:39 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 13:14:42 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 13:14:44 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 13:14:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 13:17:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 13:17:28 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 13:17:32 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 13:17:36 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:17:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:17:47 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 13:17:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 13:17:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 13:18:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 13:18:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 13:18:20 GMT
USER 1001
# Wed, 02 Feb 2022 13:18:22 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:18:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:18:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:f07957a1221172c6788544c1d5be2c025db76a8192189c7e9816319ee45224d5`  
		Last Modified: Wed, 02 Feb 2022 13:34:50 GMT  
		Size: 14.2 MB (14154738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504594bd259b50a0a43a4929a9bd06b5135bc312c12ef736c9e468376bccf17`  
		Last Modified: Wed, 02 Feb 2022 13:34:44 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0a91ef55f0eb556d7f1dbc2d5abec025223c934b73d05998afa3f130167b25`  
		Last Modified: Wed, 02 Feb 2022 13:34:44 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa0922505eedd0e6a53a1a82d98f07d8e85d431ec2a2c3bd38a54668959fee2`  
		Last Modified: Wed, 02 Feb 2022 13:34:44 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862f3b11ae60d55d8da42b76c4c95d262accaef2c36bd8954da769f89f75d8a0`  
		Last Modified: Wed, 02 Feb 2022 13:34:45 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a06a09bb6f8a75e2b2a3fd31488c92810fad3792a00260b6ed4d4cf7c459c3`  
		Last Modified: Wed, 02 Feb 2022 13:34:45 GMT  
		Size: 2.5 MB (2459343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7e914c11075ced664ee9e420175887ec3cdb1000afefaf1f95380db4139ca742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110514440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf6d4722940fd25d7e18e00d53fb2fb3ebf5cc546548acf689e6eecabb27bc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:31:48 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 05:31:48 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 05:31:48 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 05:31:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:31:48 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 05:31:49 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:31:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:31:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:32:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:32:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 05:32:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:32:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:32:01 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:32:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:32:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:32:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:32:08 GMT
USER 1001
# Wed, 02 Feb 2022 05:32:08 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:32:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:32:08 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:87898b3e11118d4555b22087ce18be3803af6a75379a4b35578d4254b6cb9796`  
		Last Modified: Wed, 02 Feb 2022 05:43:44 GMT  
		Size: 14.2 MB (14154300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e22c64bffc29b0c1f05ae6f680e70146130787d93915ccc3edecf2eea97b89`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae9936029879b0e5434e73148772ebcaf1d2dcdabd2d6487d134ed5e49f8eb8`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a613c6e9755c8568d36ae136a708f950c7c401e9181b802ad44fbb0f5673be`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d2c325811afdd268701b01df66e369940b62defd95f0ad7286cd5780bfd788`  
		Last Modified: Wed, 02 Feb 2022 05:43:41 GMT  
		Size: 10.7 KB (10650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6fdf247b898594907c5bbdaa8fdd6c479f098c66aeeb8901b50d64c02bcc7`  
		Last Modified: Wed, 02 Feb 2022 05:43:42 GMT  
		Size: 2.5 MB (2508304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:572ed41832d0182c4110ed2045d0cea3cbae5c49977439fba1f8abce70678f09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:3b6066e7885c4dc5d315a2b9e2fae4c584ac7e677c7e8ca6db10d27ff9aa0e5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178111587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007f3e5b91137bf24d925724228e203d71e98c32eb8898fee8817986b93dbb05`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:31:42 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 07 Jan 2022 07:31:42 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 07 Jan 2022 07:31:42 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Fri, 07 Jan 2022 07:31:42 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:31:43 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Fri, 07 Jan 2022 07:31:43 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:31:43 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:31:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:31:53 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:31:53 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Fri, 07 Jan 2022 07:31:53 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:31:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:31:54 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:31:55 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:31:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:32:06 GMT
USER 1001
# Fri, 07 Jan 2022 07:32:06 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43504885995bd15c4af92a25a6359972b28b014371961dd90f79d1688adc18c`  
		Last Modified: Fri, 07 Jan 2022 07:41:28 GMT  
		Size: 14.1 MB (14056166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f069e2f59a77bfcbc1d5d2f8ae152ee5965c0f63d3d579e3ea2377c612da8dd5`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164b4defa73bd9deb729b95d6e68d37f1a3c292ae7c6ee6abae9dc9ce5f489e9`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6400ed0a0c0230917df6449d849dcde3a76292f48556ce6f276e0a0cca92723`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cc8fdcb84164f33db1d71b543f85b34719d9fcd4c0575b30f8fc22502727e8`  
		Last Modified: Fri, 07 Jan 2022 07:41:24 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbd640931cdaa374c7241da9b00014a7740a80fc7a15facc8231df8a65917ac`  
		Last Modified: Fri, 07 Jan 2022 07:41:25 GMT  
		Size: 5.6 MB (5642065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:23bc0444d7a484b9053476bc9864ba67e81bcfe4da3be1c46389e068318b8dcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181117351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183293fb6daeb1d7ea8b4f880be600a22cf17d00e3b736793c8c05ba7b6caaef`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:11:04 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 13:11:07 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 13:11:09 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 13:11:13 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 13:11:16 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 13:11:19 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 13:11:21 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 13:13:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 13:13:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 13:13:21 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 13:13:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 13:13:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 13:13:35 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 13:13:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 13:13:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 13:14:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 13:14:10 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 13:14:13 GMT
USER 1001
# Wed, 02 Feb 2022 13:14:15 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 13:14:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 13:14:18 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0008763388a9b63fabf4b13a6fec7a09a446d3282608474c642537c4904eaba5`  
		Last Modified: Wed, 02 Feb 2022 13:34:36 GMT  
		Size: 14.1 MB (14056148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feefa873c251180b540857621a8f0d44afe142654c3acbf2009e63a060fadf68`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39d715958173ac01bf793eef34a43223c968ee44f382c60af538e0dec45b5f3`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bea67f0ce83d7df3600b994d95ee04b0d319290d4889edc8e17cc0b6df55f8`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cdf9e22417e1ed70bfc90c84696bf0deedb986535f38c1dc83dd25c47e213b`  
		Last Modified: Wed, 02 Feb 2022 13:34:31 GMT  
		Size: 10.7 KB (10661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cad774cff61a16f94c5f1737cc74eb758bc020d72345542762618a29cf8bdf7`  
		Last Modified: Wed, 02 Feb 2022 13:34:32 GMT  
		Size: 5.3 MB (5264168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f211d60338699ba74e6e058391ebf76366d62f76a701563ab423ab3eecced1ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173614961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bb46d1190d423cb9390b4ddc4d881001d92806009fa3ee91d4f7ce15d4513d`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:31:16 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 02 Feb 2022 05:31:16 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 02 Feb 2022 05:31:16 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 02 Feb 2022 05:31:16 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:31:17 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 02 Feb 2022 05:31:17 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:31:17 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:31:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:31:30 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:31:30 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 02 Feb 2022 05:31:30 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:31:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:31:31 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:31:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:31:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:31:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:31:39 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:31:39 GMT
USER 1001
# Wed, 02 Feb 2022 05:31:39 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:31:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:31:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85402617352148106bf0a09a99cb07af7ffa2e47cafeb72b21e8526352180ec9`  
		Last Modified: Wed, 02 Feb 2022 05:43:37 GMT  
		Size: 14.1 MB (14055651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2cb196bf0e4bd26f0cd142b60a22b21b3aa9b89ef35dccfac1e171be77a687`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca286209f84c9c4eddb8358a213aca4ba7c55c9f33ebe205b5edd6dbe6122fb`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91066126bb9ae5d636277fe1a07f98dced5477bcec7aa9225907ee424dedb9d`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e37f2f3d254b346894c67e6524cbd8ac6d83ff75deb3c24d7779a49b5017f9`  
		Last Modified: Wed, 02 Feb 2022 05:43:34 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f9af41e41b78737610210688142a4747597f12eb7fd06c3dc8ff88b5aad40a`  
		Last Modified: Wed, 02 Feb 2022 05:43:35 GMT  
		Size: 5.8 MB (5759525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:a20e501fc6f0c0557bafdab4fdafc1251da5157577c2d2ab22ca4656262a1353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.1-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:989369b2a4e8d77615243a3b9e044567294497ce11bcc2f2f8626a9cf5c8eec5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.0 MB (399021744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e0284825c9597dc9327c3a33bd4d2d3946108f9dfc354c322dc1f6eec38620`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:32:58 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:32:59 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:32:59 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:32:59 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:33:00 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:33:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:33:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:33:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:33:10 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:33:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:33:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:33:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:33:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:33:20 GMT
USER 1001
# Tue, 01 Feb 2022 02:33:20 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:33:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:33:21 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:33:28 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:33:28 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:37:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:37:18 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:37:53 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:5e1dcd3d2744a39ecf8f1eb95e552c9539b5c0dc1494e733c3e3d623e4238921`  
		Last Modified: Tue, 01 Feb 2022 02:48:10 GMT  
		Size: 14.2 MB (14228744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264689484e10222b810a9835bd73fca46d470352f1409281894bd47289ca2de`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6458b29c6d007c2815431fed0e357875ba770119f91e2d3440ca2b65aaef9`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3707d42323ee4f32e04d5c800e6e75b4353c598aca35c595ce26cae4056a50`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff56ac88d4d78ee0500eed83f0de20125d9124f0b03822f6d043930dbe28face`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 10.6 KB (10644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3346f7e9502060f9168a88d25c05ce2e278b2295421bf05d3cf041302d5d43b`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 2.5 MB (2497252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a947777feab474ef0ceccde5aca5faf14ab4e8c6013194a557e01f7b0ed8029c`  
		Last Modified: Tue, 01 Feb 2022 02:48:38 GMT  
		Size: 271.1 MB (271128369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c5297ec70855b04fe3d1433579b72db78b9a374f71689ea47e87997388596`  
		Last Modified: Tue, 01 Feb 2022 02:48:23 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9304a1202c728ce8a56336257031b34f5138b71ab51a37be53ab93d1a9c17e7`  
		Last Modified: Tue, 01 Feb 2022 02:48:26 GMT  
		Size: 14.4 MB (14431308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:7dd2e4d5b683de6ad413301555503c929bd27b82f9e01dc297631721d6aed740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.5 MB (402537956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d9c3def7ba8ecd1a28b662e1ef06b54758290bad23b53f568a3f317a9c5d6a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:30:09 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:30:12 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:30:17 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:30:20 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:30:22 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:30:23 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:30:25 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:34:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:34:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:34:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:34:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:34:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:34:26 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:34:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:34:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:34:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:34:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 12:34:56 GMT
USER 1001
# Wed, 02 Feb 2022 12:34:59 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:35:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:35:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 12:41:23 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:41:24 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 12:46:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 12:46:28 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 12:47:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:c629adcc50d21cebe396ee7b5026dd3d69f6029335c22b737b035812319c8c1e`  
		Last Modified: Wed, 02 Feb 2022 13:30:34 GMT  
		Size: 14.2 MB (14229389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59f56b86c301261a2a803a6d67d5174698150d320c3efe5e91e15509697dd8f`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21af9b4ba609b521be416c2a168614b33b85d6525b955a52af1489367c408e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc61794979abd71755b503170df22260137800fe704cc8234b27166c41cd762e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2ae613b2a8041310d1994b1da58d012e404eb8c62eac7f661774f867b0895`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbbe136d84c625633722280da81510ed9072b0456f4e6bc0a4c0c9047c9b141`  
		Last Modified: Wed, 02 Feb 2022 13:30:27 GMT  
		Size: 2.5 MB (2479493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746ae46d0c7af13cf4096196a01d682b7e519f4a1a6091d7614ff2f31a76b6ed`  
		Last Modified: Wed, 02 Feb 2022 13:32:37 GMT  
		Size: 271.1 MB (271128814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b83815b5b9cdcc4e27a0463a270ef31e4582097010c3a56466de0996105180`  
		Last Modified: Wed, 02 Feb 2022 13:32:00 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17504d9b825211d6cbcc4e2602ea9dd63923f3d6cae25d69c9dcae4d247aa120`  
		Last Modified: Wed, 02 Feb 2022 13:32:03 GMT  
		Size: 12.5 MB (12512994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:21456c4862b12254a28ea0f045cafd4e4714bdc04d166244b2370eb13bfa08da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396207519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2707623fd842c0c5a900daeb11819d0adf2fd72862379a297f42c77d944a5f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:55 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:55 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:55 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:55 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:10:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:10:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:10:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:10:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:10:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:10:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:10:15 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:10:16 GMT
USER 1001
# Wed, 02 Feb 2022 05:10:16 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:10:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:10:16 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:15:33 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:15:33 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:19:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:19:54 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:20:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:c77602311a93edd5a58c83bbaf902ef7b03f2bee21e46360e6f3ad59f4045d23`  
		Last Modified: Wed, 02 Feb 2022 05:41:50 GMT  
		Size: 14.2 MB (14228938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab4fe7a0d81db18bac0038775ade0036f6ecd92c6573021d04cf632b6a183f`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee683ad878b74455936766919bde75a7517845a605dce5e6d20674d79b57b5b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f2fdd0c8a61e80f6ccf93143100796e740ab083de3f887522ab583411006a9`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc16640575440e02ab2598d69e93ffbc294b0bfe275d3eda05a77f2705a5d4b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787acc60dd91e6d838b87186e5d88fbde358467834865f7b7c3d87493f87442b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 2.5 MB (2500548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4221cb325e58e4b6fe30954995b62cbbcf654da8a50bf2bb986475df1f8bdf4e`  
		Last Modified: Wed, 02 Feb 2022 05:42:26 GMT  
		Size: 271.1 MB (271128725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e4965a56942f52dcdd9d8e5bb8c0768c1659f58574c0347a5e61010cd66f4`  
		Last Modified: Wed, 02 Feb 2022 05:42:15 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56a24659b98329441cae4047d98197c5f263de9028dbd89bcc4d17d9efb0db2`  
		Last Modified: Wed, 02 Feb 2022 05:42:16 GMT  
		Size: 14.5 MB (14496528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:32d04e4d823f6682982326360f3fa4caeeb5b235cd665ba05ef6403a6ef74cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.1-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:1523d1425988c2bd44ee54cfbe65d217eaa32202eed52014ba74294e22a59c68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.6 MB (465578785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e79631b682f29c4f03e4b297dc65a50ae4e26fda4d8564068ef547f39d9e982`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:28:52 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:28:53 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:28:53 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:28:53 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:28:53 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:29:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:29:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:29:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:29:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:29:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:29:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:29:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:29:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:29:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:29:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:29:33 GMT
USER 1001
# Tue, 25 Jan 2022 23:29:33 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:29:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:29:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 23:30:08 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 23:30:08 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 23:33:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 23:33:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 23:34:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684cbf0832df4654ac666b7af4422d156c1e5ebc781c84a861b9876fd6719ad9`  
		Last Modified: Tue, 25 Jan 2022 23:40:12 GMT  
		Size: 14.1 MB (14130816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdd64484cfa06e57ebfba3acc22e4ec6779557b52d55a3fafad7a4ed4eae8e9`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95128698b2f7eb1a6e3dd47b30695b0ebac941fce5b5790f2b1b49987ec29a5a`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16d0044e066e31dbad560d64450bf3b182e65d9f913823b5066aa3c79c39c0c`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17802f8569a2d6741632ab087d9461ff3aacb49e8b260ad622e79cd042127bfc`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7a4b18294b82e0fd276930e5f828a812c3101ffbced931e44c4a359697634`  
		Last Modified: Tue, 25 Jan 2022 23:40:10 GMT  
		Size: 5.7 MB (5655523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50e52c6aa148d7c7b338b00e0c24b0d4a815d021bfb941913df0b0851d5c4f1`  
		Last Modified: Tue, 25 Jan 2022 23:40:52 GMT  
		Size: 271.1 MB (271128666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35be19483cac5f6a010f8262cb95240db20619ec93bdf32cbfaf7b36d4c5807`  
		Last Modified: Tue, 25 Jan 2022 23:40:39 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b92982762035daabfc5fb8d0bff64015300723be82b825ff85c93af44c9968`  
		Last Modified: Tue, 25 Jan 2022 23:40:42 GMT  
		Size: 16.2 MB (16249449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:90866fcb374315d224ccd6f53dd26b2166e79bda95726a25dc3373fea2a25279
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466059188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f21f2cb7cf9c1516aa78f39e4414381affc89efb0f819cfbd4f727f0097e35f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:25:26 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:25:29 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:25:31 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:25:32 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:25:36 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:25:37 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:25:40 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:28:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:28:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:28:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:28:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:28:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:28:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:28:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:29:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:29:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:29:30 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:29:32 GMT
USER 1001
# Wed, 02 Feb 2022 12:29:35 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:29:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:29:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 12:35:15 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:35:17 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 12:40:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 12:40:17 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 12:41:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bdd8addeaf2c0b6bb30d08a19e51130187d8e5e24e046eced8cf481f611bf8`  
		Last Modified: Wed, 02 Feb 2022 13:30:18 GMT  
		Size: 14.1 MB (14130794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4224b13f14b349ab121fc8921d706e872baf263faf40b5569a0be3a90dc641`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9540b5678c1e636d2cddfa7fb7e893576b7b68d50b52dfa5aace97d09abf9c08`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426b46c2de6c5cab17c57667b78bc99a62b010696889b3a733865e5fa307038b`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c0353910905dbcb8e90ac0424838bad1bc1490244ec658b67125e339bb37e5`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b548213c4a4358f74e22dbc35c05cfbf76610870900e8cb282aefe4d318c9b7`  
		Last Modified: Wed, 02 Feb 2022 13:30:08 GMT  
		Size: 5.3 MB (5255386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a339184bb89b8167f43d5fc1a94213349bc819c866d54b59432d8d6a7cdc2`  
		Last Modified: Wed, 02 Feb 2022 13:31:48 GMT  
		Size: 271.1 MB (271129407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d05420f0f7365a419a31f6712d794d606bcf351ece8f9a04f38bb297c5496de`  
		Last Modified: Wed, 02 Feb 2022 13:30:43 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acb9725035238f7f7d7fee9a0a0032aac45f265c569375e104f1bf01a6b45a`  
		Last Modified: Wed, 02 Feb 2022 13:30:46 GMT  
		Size: 13.7 MB (13745624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:21d37155d493324cc388d37767a473ed148955b7c9a9ed7cd65305130e60ed8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460722956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4898ad2a7e8479a21d4f806f585f787645a90d7eed83919e40a7ef466e4ba2d7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:27 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:28 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:28 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:28 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:09:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:09:40 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:09:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:09:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:09:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:09:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:09:48 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:48 GMT
USER 1001
# Wed, 02 Feb 2022 05:09:48 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:09:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:09:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:10:23 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:10:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:14:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:14:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:15:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8d99305c3aacb5d4b51d664499bec25524ed7b6b2f51b72246d1fbde756669`  
		Last Modified: Wed, 02 Feb 2022 05:41:43 GMT  
		Size: 14.1 MB (14130296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735955845bdd39fb6bec511d39f6a3f91fdcd129d4673efceeeffb1fd71f543`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff820f8badf1b036673f852841f1f66f70fae3fdd930367b45e59622bee4be5`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c96f2aa98216b37f007ab4fc482783fbda6c1cb4f35278749e9d6cf21fb829`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe1b767832f1415d9e4b05ee726a113eb14f1c5ed1942644826961a7de2bb`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2225e04c87a6e2ef8f45524c9929cac9342e4c8b5c37109aa9a54421ddc280bd`  
		Last Modified: Wed, 02 Feb 2022 05:41:42 GMT  
		Size: 5.7 MB (5722410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba19544da9e3e1e528ba844c095f75be212ea1ef20cf6f9930b1dd6722d0df5d`  
		Last Modified: Wed, 02 Feb 2022 05:42:07 GMT  
		Size: 271.1 MB (271128976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf5b3e381e121e19f39fa92edec3c96d222f34fb75effb09082f1ddad0ac796`  
		Last Modified: Wed, 02 Feb 2022 05:41:56 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c8b74b60a36baf6ce0e1ee249c6693f04d466539db0029b0a623a6bc802def`  
		Last Modified: Wed, 02 Feb 2022 05:41:58 GMT  
		Size: 15.9 MB (15940538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:9050197bc9253da1306a219e5c38dc51ca41f3302d7888c9d05f94742e07a31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.1-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9a2d38540ca0b1dc0bb591b3487185110f0a07e783af525c5b86c15a28a0330d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113461123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284de8c381ad1b2a8189a13739a93a66dcf2fdab83b49943f9a97acf69e22b53`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:32:58 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:32:59 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:32:59 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:32:59 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:33:00 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:33:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:33:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:33:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:33:10 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:33:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:33:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:33:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:33:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:33:20 GMT
USER 1001
# Tue, 01 Feb 2022 02:33:20 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:33:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:33:21 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:5e1dcd3d2744a39ecf8f1eb95e552c9539b5c0dc1494e733c3e3d623e4238921`  
		Last Modified: Tue, 01 Feb 2022 02:48:10 GMT  
		Size: 14.2 MB (14228744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264689484e10222b810a9835bd73fca46d470352f1409281894bd47289ca2de`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6458b29c6d007c2815431fed0e357875ba770119f91e2d3440ca2b65aaef9`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3707d42323ee4f32e04d5c800e6e75b4353c598aca35c595ce26cae4056a50`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff56ac88d4d78ee0500eed83f0de20125d9124f0b03822f6d043930dbe28face`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 10.6 KB (10644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3346f7e9502060f9168a88d25c05ce2e278b2295421bf05d3cf041302d5d43b`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 2.5 MB (2497252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c1eb3c484964b48f70fbec011730ccc0b26dd7e2aa80cb32cc5eee87966659f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118895201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70835d223bdc357e86599ea85d6e089d4e92b58d9b17241361527eab2ea049c6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:30:09 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:30:12 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:30:17 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:30:20 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:30:22 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:30:23 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:30:25 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:34:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:34:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:34:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:34:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:34:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:34:26 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:34:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:34:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:34:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:34:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 12:34:56 GMT
USER 1001
# Wed, 02 Feb 2022 12:34:59 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:35:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:35:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:c629adcc50d21cebe396ee7b5026dd3d69f6029335c22b737b035812319c8c1e`  
		Last Modified: Wed, 02 Feb 2022 13:30:34 GMT  
		Size: 14.2 MB (14229389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59f56b86c301261a2a803a6d67d5174698150d320c3efe5e91e15509697dd8f`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21af9b4ba609b521be416c2a168614b33b85d6525b955a52af1489367c408e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc61794979abd71755b503170df22260137800fe704cc8234b27166c41cd762e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2ae613b2a8041310d1994b1da58d012e404eb8c62eac7f661774f867b0895`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbbe136d84c625633722280da81510ed9072b0456f4e6bc0a4c0c9047c9b141`  
		Last Modified: Wed, 02 Feb 2022 13:30:27 GMT  
		Size: 2.5 MB (2479493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:45b3564f7ef45bb9b96bfe3539da65b12a5d1749543910e9da075cf419fd689b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110581327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47c6d5b432741525623111529c7ab9af1e78b40da6dc471ef61af9cab008459`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:55 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:55 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:55 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:55 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:10:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:10:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:10:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:10:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:10:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:10:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:10:15 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:10:16 GMT
USER 1001
# Wed, 02 Feb 2022 05:10:16 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:10:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:10:16 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:c77602311a93edd5a58c83bbaf902ef7b03f2bee21e46360e6f3ad59f4045d23`  
		Last Modified: Wed, 02 Feb 2022 05:41:50 GMT  
		Size: 14.2 MB (14228938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab4fe7a0d81db18bac0038775ade0036f6ecd92c6573021d04cf632b6a183f`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee683ad878b74455936766919bde75a7517845a605dce5e6d20674d79b57b5b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f2fdd0c8a61e80f6ccf93143100796e740ab083de3f887522ab583411006a9`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc16640575440e02ab2598d69e93ffbc294b0bfe275d3eda05a77f2705a5d4b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787acc60dd91e6d838b87186e5d88fbde358467834865f7b7c3d87493f87442b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 2.5 MB (2500548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:df29418536ad079dcc92e83d4e51b5465ce1d1f88c95652c71da8dbba2957712
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.1-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:961618ef82ebf30c092252c253ae435cb91cf75dc2a3f17bb32e8d793c942514
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178199725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d4ee5f5e435da4e201d6562fea246183aeb52bd6121f8c461fee20023c9591`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:28:52 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:28:53 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:28:53 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:28:53 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:28:53 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:29:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:29:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:29:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:29:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:29:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:29:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:29:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:29:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:29:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:29:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:29:33 GMT
USER 1001
# Tue, 25 Jan 2022 23:29:33 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:29:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:29:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684cbf0832df4654ac666b7af4422d156c1e5ebc781c84a861b9876fd6719ad9`  
		Last Modified: Tue, 25 Jan 2022 23:40:12 GMT  
		Size: 14.1 MB (14130816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdd64484cfa06e57ebfba3acc22e4ec6779557b52d55a3fafad7a4ed4eae8e9`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95128698b2f7eb1a6e3dd47b30695b0ebac941fce5b5790f2b1b49987ec29a5a`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16d0044e066e31dbad560d64450bf3b182e65d9f913823b5066aa3c79c39c0c`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17802f8569a2d6741632ab087d9461ff3aacb49e8b260ad622e79cd042127bfc`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7a4b18294b82e0fd276930e5f828a812c3101ffbced931e44c4a359697634`  
		Last Modified: Tue, 25 Jan 2022 23:40:10 GMT  
		Size: 5.7 MB (5655523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ace7dd34608370768a4ea53ef6076e18ca80bda3b8b733092b47ea68d0432076
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.2 MB (181183213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:628a656de15e034b9dbaadae2e9efe959f808d1482d5a3ba2c07b812e360c349`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:25:26 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:25:29 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:25:31 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:25:32 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:25:36 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:25:37 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:25:40 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:28:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:28:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:28:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:28:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:28:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:28:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:28:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:29:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:29:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:29:30 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:29:32 GMT
USER 1001
# Wed, 02 Feb 2022 12:29:35 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:29:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:29:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bdd8addeaf2c0b6bb30d08a19e51130187d8e5e24e046eced8cf481f611bf8`  
		Last Modified: Wed, 02 Feb 2022 13:30:18 GMT  
		Size: 14.1 MB (14130794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4224b13f14b349ab121fc8921d706e872baf263faf40b5569a0be3a90dc641`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9540b5678c1e636d2cddfa7fb7e893576b7b68d50b52dfa5aace97d09abf9c08`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426b46c2de6c5cab17c57667b78bc99a62b010696889b3a733865e5fa307038b`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c0353910905dbcb8e90ac0424838bad1bc1490244ec658b67125e339bb37e5`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b548213c4a4358f74e22dbc35c05cfbf76610870900e8cb282aefe4d318c9b7`  
		Last Modified: Wed, 02 Feb 2022 13:30:08 GMT  
		Size: 5.3 MB (5255386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0eaa348875aaa74f5261f11019fcc068064796a06f6fd1b8501f8753674ec7dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173652495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24bd838ca997e0744c8926327d5d21c7c89f4234d4c399da6a3aa45df03fee1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:27 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:28 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:28 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:28 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:09:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:09:40 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:09:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:09:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:09:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:09:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:09:48 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:48 GMT
USER 1001
# Wed, 02 Feb 2022 05:09:48 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:09:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:09:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8d99305c3aacb5d4b51d664499bec25524ed7b6b2f51b72246d1fbde756669`  
		Last Modified: Wed, 02 Feb 2022 05:41:43 GMT  
		Size: 14.1 MB (14130296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735955845bdd39fb6bec511d39f6a3f91fdcd129d4673efceeeffb1fd71f543`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff820f8badf1b036673f852841f1f66f70fae3fdd930367b45e59622bee4be5`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c96f2aa98216b37f007ab4fc482783fbda6c1cb4f35278749e9d6cf21fb829`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe1b767832f1415d9e4b05ee726a113eb14f1c5ed1942644826961a7de2bb`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2225e04c87a6e2ef8f45524c9929cac9342e4c8b5c37109aa9a54421ddc280bd`  
		Last Modified: Wed, 02 Feb 2022 05:41:42 GMT  
		Size: 5.7 MB (5722410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:32d04e4d823f6682982326360f3fa4caeeb5b235cd665ba05ef6403a6ef74cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:1523d1425988c2bd44ee54cfbe65d217eaa32202eed52014ba74294e22a59c68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.6 MB (465578785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e79631b682f29c4f03e4b297dc65a50ae4e26fda4d8564068ef547f39d9e982`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:28:52 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:28:53 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:28:53 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:28:53 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:28:53 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:29:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:29:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:29:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:29:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:29:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:29:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:29:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:29:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:29:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:29:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:29:33 GMT
USER 1001
# Tue, 25 Jan 2022 23:29:33 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:29:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:29:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 23:30:08 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 23:30:08 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 23:33:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 23:33:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 23:34:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684cbf0832df4654ac666b7af4422d156c1e5ebc781c84a861b9876fd6719ad9`  
		Last Modified: Tue, 25 Jan 2022 23:40:12 GMT  
		Size: 14.1 MB (14130816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdd64484cfa06e57ebfba3acc22e4ec6779557b52d55a3fafad7a4ed4eae8e9`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95128698b2f7eb1a6e3dd47b30695b0ebac941fce5b5790f2b1b49987ec29a5a`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16d0044e066e31dbad560d64450bf3b182e65d9f913823b5066aa3c79c39c0c`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17802f8569a2d6741632ab087d9461ff3aacb49e8b260ad622e79cd042127bfc`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7a4b18294b82e0fd276930e5f828a812c3101ffbced931e44c4a359697634`  
		Last Modified: Tue, 25 Jan 2022 23:40:10 GMT  
		Size: 5.7 MB (5655523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50e52c6aa148d7c7b338b00e0c24b0d4a815d021bfb941913df0b0851d5c4f1`  
		Last Modified: Tue, 25 Jan 2022 23:40:52 GMT  
		Size: 271.1 MB (271128666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35be19483cac5f6a010f8262cb95240db20619ec93bdf32cbfaf7b36d4c5807`  
		Last Modified: Tue, 25 Jan 2022 23:40:39 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b92982762035daabfc5fb8d0bff64015300723be82b825ff85c93af44c9968`  
		Last Modified: Tue, 25 Jan 2022 23:40:42 GMT  
		Size: 16.2 MB (16249449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:90866fcb374315d224ccd6f53dd26b2166e79bda95726a25dc3373fea2a25279
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466059188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f21f2cb7cf9c1516aa78f39e4414381affc89efb0f819cfbd4f727f0097e35f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:25:26 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:25:29 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:25:31 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:25:32 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:25:36 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:25:37 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:25:40 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:28:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:28:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:28:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:28:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:28:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:28:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:28:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:29:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:29:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:29:30 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:29:32 GMT
USER 1001
# Wed, 02 Feb 2022 12:29:35 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:29:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:29:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 12:35:15 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:35:17 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 12:40:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 12:40:17 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 12:41:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bdd8addeaf2c0b6bb30d08a19e51130187d8e5e24e046eced8cf481f611bf8`  
		Last Modified: Wed, 02 Feb 2022 13:30:18 GMT  
		Size: 14.1 MB (14130794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4224b13f14b349ab121fc8921d706e872baf263faf40b5569a0be3a90dc641`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9540b5678c1e636d2cddfa7fb7e893576b7b68d50b52dfa5aace97d09abf9c08`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426b46c2de6c5cab17c57667b78bc99a62b010696889b3a733865e5fa307038b`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c0353910905dbcb8e90ac0424838bad1bc1490244ec658b67125e339bb37e5`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b548213c4a4358f74e22dbc35c05cfbf76610870900e8cb282aefe4d318c9b7`  
		Last Modified: Wed, 02 Feb 2022 13:30:08 GMT  
		Size: 5.3 MB (5255386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a339184bb89b8167f43d5fc1a94213349bc819c866d54b59432d8d6a7cdc2`  
		Last Modified: Wed, 02 Feb 2022 13:31:48 GMT  
		Size: 271.1 MB (271129407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d05420f0f7365a419a31f6712d794d606bcf351ece8f9a04f38bb297c5496de`  
		Last Modified: Wed, 02 Feb 2022 13:30:43 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acb9725035238f7f7d7fee9a0a0032aac45f265c569375e104f1bf01a6b45a`  
		Last Modified: Wed, 02 Feb 2022 13:30:46 GMT  
		Size: 13.7 MB (13745624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:21d37155d493324cc388d37767a473ed148955b7c9a9ed7cd65305130e60ed8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460722956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4898ad2a7e8479a21d4f806f585f787645a90d7eed83919e40a7ef466e4ba2d7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:27 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:28 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:28 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:28 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:09:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:09:40 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:09:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:09:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:09:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:09:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:09:48 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:48 GMT
USER 1001
# Wed, 02 Feb 2022 05:09:48 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:09:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:09:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:10:23 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:10:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:14:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:14:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:15:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8d99305c3aacb5d4b51d664499bec25524ed7b6b2f51b72246d1fbde756669`  
		Last Modified: Wed, 02 Feb 2022 05:41:43 GMT  
		Size: 14.1 MB (14130296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735955845bdd39fb6bec511d39f6a3f91fdcd129d4673efceeeffb1fd71f543`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff820f8badf1b036673f852841f1f66f70fae3fdd930367b45e59622bee4be5`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c96f2aa98216b37f007ab4fc482783fbda6c1cb4f35278749e9d6cf21fb829`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe1b767832f1415d9e4b05ee726a113eb14f1c5ed1942644826961a7de2bb`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2225e04c87a6e2ef8f45524c9929cac9342e4c8b5c37109aa9a54421ddc280bd`  
		Last Modified: Wed, 02 Feb 2022 05:41:42 GMT  
		Size: 5.7 MB (5722410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba19544da9e3e1e528ba844c095f75be212ea1ef20cf6f9930b1dd6722d0df5d`  
		Last Modified: Wed, 02 Feb 2022 05:42:07 GMT  
		Size: 271.1 MB (271128976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf5b3e381e121e19f39fa92edec3c96d222f34fb75effb09082f1ddad0ac796`  
		Last Modified: Wed, 02 Feb 2022 05:41:56 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c8b74b60a36baf6ce0e1ee249c6693f04d466539db0029b0a623a6bc802def`  
		Last Modified: Wed, 02 Feb 2022 05:41:58 GMT  
		Size: 15.9 MB (15940538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:a20e501fc6f0c0557bafdab4fdafc1251da5157577c2d2ab22ca4656262a1353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:989369b2a4e8d77615243a3b9e044567294497ce11bcc2f2f8626a9cf5c8eec5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.0 MB (399021744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e0284825c9597dc9327c3a33bd4d2d3946108f9dfc354c322dc1f6eec38620`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:32:58 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:32:59 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:32:59 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:32:59 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:33:00 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:33:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:33:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:33:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:33:10 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:33:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:33:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:33:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:33:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:33:20 GMT
USER 1001
# Tue, 01 Feb 2022 02:33:20 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:33:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:33:21 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:33:28 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:33:28 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:37:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:37:18 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:37:53 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:5e1dcd3d2744a39ecf8f1eb95e552c9539b5c0dc1494e733c3e3d623e4238921`  
		Last Modified: Tue, 01 Feb 2022 02:48:10 GMT  
		Size: 14.2 MB (14228744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264689484e10222b810a9835bd73fca46d470352f1409281894bd47289ca2de`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6458b29c6d007c2815431fed0e357875ba770119f91e2d3440ca2b65aaef9`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3707d42323ee4f32e04d5c800e6e75b4353c598aca35c595ce26cae4056a50`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff56ac88d4d78ee0500eed83f0de20125d9124f0b03822f6d043930dbe28face`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 10.6 KB (10644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3346f7e9502060f9168a88d25c05ce2e278b2295421bf05d3cf041302d5d43b`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 2.5 MB (2497252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a947777feab474ef0ceccde5aca5faf14ab4e8c6013194a557e01f7b0ed8029c`  
		Last Modified: Tue, 01 Feb 2022 02:48:38 GMT  
		Size: 271.1 MB (271128369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c5297ec70855b04fe3d1433579b72db78b9a374f71689ea47e87997388596`  
		Last Modified: Tue, 01 Feb 2022 02:48:23 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9304a1202c728ce8a56336257031b34f5138b71ab51a37be53ab93d1a9c17e7`  
		Last Modified: Tue, 01 Feb 2022 02:48:26 GMT  
		Size: 14.4 MB (14431308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:7dd2e4d5b683de6ad413301555503c929bd27b82f9e01dc297631721d6aed740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.5 MB (402537956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d9c3def7ba8ecd1a28b662e1ef06b54758290bad23b53f568a3f317a9c5d6a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:30:09 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:30:12 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:30:17 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:30:20 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:30:22 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:30:23 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:30:25 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:34:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:34:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:34:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:34:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:34:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:34:26 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:34:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:34:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:34:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:34:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 12:34:56 GMT
USER 1001
# Wed, 02 Feb 2022 12:34:59 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:35:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:35:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 12:41:23 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:41:24 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 12:46:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 12:46:28 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 12:47:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:c629adcc50d21cebe396ee7b5026dd3d69f6029335c22b737b035812319c8c1e`  
		Last Modified: Wed, 02 Feb 2022 13:30:34 GMT  
		Size: 14.2 MB (14229389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59f56b86c301261a2a803a6d67d5174698150d320c3efe5e91e15509697dd8f`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21af9b4ba609b521be416c2a168614b33b85d6525b955a52af1489367c408e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc61794979abd71755b503170df22260137800fe704cc8234b27166c41cd762e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2ae613b2a8041310d1994b1da58d012e404eb8c62eac7f661774f867b0895`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbbe136d84c625633722280da81510ed9072b0456f4e6bc0a4c0c9047c9b141`  
		Last Modified: Wed, 02 Feb 2022 13:30:27 GMT  
		Size: 2.5 MB (2479493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746ae46d0c7af13cf4096196a01d682b7e519f4a1a6091d7614ff2f31a76b6ed`  
		Last Modified: Wed, 02 Feb 2022 13:32:37 GMT  
		Size: 271.1 MB (271128814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b83815b5b9cdcc4e27a0463a270ef31e4582097010c3a56466de0996105180`  
		Last Modified: Wed, 02 Feb 2022 13:32:00 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17504d9b825211d6cbcc4e2602ea9dd63923f3d6cae25d69c9dcae4d247aa120`  
		Last Modified: Wed, 02 Feb 2022 13:32:03 GMT  
		Size: 12.5 MB (12512994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:21456c4862b12254a28ea0f045cafd4e4714bdc04d166244b2370eb13bfa08da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396207519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2707623fd842c0c5a900daeb11819d0adf2fd72862379a297f42c77d944a5f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:55 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:55 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:55 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:55 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:10:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:10:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:10:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:10:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:10:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:10:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:10:15 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:10:16 GMT
USER 1001
# Wed, 02 Feb 2022 05:10:16 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:10:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:10:16 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:15:33 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:15:33 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:19:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:19:54 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:20:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:c77602311a93edd5a58c83bbaf902ef7b03f2bee21e46360e6f3ad59f4045d23`  
		Last Modified: Wed, 02 Feb 2022 05:41:50 GMT  
		Size: 14.2 MB (14228938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab4fe7a0d81db18bac0038775ade0036f6ecd92c6573021d04cf632b6a183f`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee683ad878b74455936766919bde75a7517845a605dce5e6d20674d79b57b5b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f2fdd0c8a61e80f6ccf93143100796e740ab083de3f887522ab583411006a9`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc16640575440e02ab2598d69e93ffbc294b0bfe275d3eda05a77f2705a5d4b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787acc60dd91e6d838b87186e5d88fbde358467834865f7b7c3d87493f87442b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 2.5 MB (2500548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4221cb325e58e4b6fe30954995b62cbbcf654da8a50bf2bb986475df1f8bdf4e`  
		Last Modified: Wed, 02 Feb 2022 05:42:26 GMT  
		Size: 271.1 MB (271128725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e4965a56942f52dcdd9d8e5bb8c0768c1659f58574c0347a5e61010cd66f4`  
		Last Modified: Wed, 02 Feb 2022 05:42:15 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56a24659b98329441cae4047d98197c5f263de9028dbd89bcc4d17d9efb0db2`  
		Last Modified: Wed, 02 Feb 2022 05:42:16 GMT  
		Size: 14.5 MB (14496528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:df29418536ad079dcc92e83d4e51b5465ce1d1f88c95652c71da8dbba2957712
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:961618ef82ebf30c092252c253ae435cb91cf75dc2a3f17bb32e8d793c942514
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178199725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d4ee5f5e435da4e201d6562fea246183aeb52bd6121f8c461fee20023c9591`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:28:52 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:28:53 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:28:53 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:28:53 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:28:53 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:29:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:29:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:29:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:29:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:29:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:29:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:29:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:29:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:29:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:29:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:29:33 GMT
USER 1001
# Tue, 25 Jan 2022 23:29:33 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:29:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:29:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684cbf0832df4654ac666b7af4422d156c1e5ebc781c84a861b9876fd6719ad9`  
		Last Modified: Tue, 25 Jan 2022 23:40:12 GMT  
		Size: 14.1 MB (14130816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdd64484cfa06e57ebfba3acc22e4ec6779557b52d55a3fafad7a4ed4eae8e9`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95128698b2f7eb1a6e3dd47b30695b0ebac941fce5b5790f2b1b49987ec29a5a`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16d0044e066e31dbad560d64450bf3b182e65d9f913823b5066aa3c79c39c0c`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17802f8569a2d6741632ab087d9461ff3aacb49e8b260ad622e79cd042127bfc`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7a4b18294b82e0fd276930e5f828a812c3101ffbced931e44c4a359697634`  
		Last Modified: Tue, 25 Jan 2022 23:40:10 GMT  
		Size: 5.7 MB (5655523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ace7dd34608370768a4ea53ef6076e18ca80bda3b8b733092b47ea68d0432076
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.2 MB (181183213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:628a656de15e034b9dbaadae2e9efe959f808d1482d5a3ba2c07b812e360c349`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:25:26 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:25:29 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:25:31 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:25:32 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:25:36 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:25:37 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:25:40 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:28:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:28:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:28:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:28:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:28:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:28:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:28:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:29:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:29:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:29:30 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:29:32 GMT
USER 1001
# Wed, 02 Feb 2022 12:29:35 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:29:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:29:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bdd8addeaf2c0b6bb30d08a19e51130187d8e5e24e046eced8cf481f611bf8`  
		Last Modified: Wed, 02 Feb 2022 13:30:18 GMT  
		Size: 14.1 MB (14130794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4224b13f14b349ab121fc8921d706e872baf263faf40b5569a0be3a90dc641`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9540b5678c1e636d2cddfa7fb7e893576b7b68d50b52dfa5aace97d09abf9c08`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426b46c2de6c5cab17c57667b78bc99a62b010696889b3a733865e5fa307038b`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c0353910905dbcb8e90ac0424838bad1bc1490244ec658b67125e339bb37e5`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b548213c4a4358f74e22dbc35c05cfbf76610870900e8cb282aefe4d318c9b7`  
		Last Modified: Wed, 02 Feb 2022 13:30:08 GMT  
		Size: 5.3 MB (5255386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0eaa348875aaa74f5261f11019fcc068064796a06f6fd1b8501f8753674ec7dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173652495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24bd838ca997e0744c8926327d5d21c7c89f4234d4c399da6a3aa45df03fee1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:27 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:28 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:28 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:28 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:09:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:09:40 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:09:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:09:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:09:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:09:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:09:48 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:48 GMT
USER 1001
# Wed, 02 Feb 2022 05:09:48 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:09:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:09:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8d99305c3aacb5d4b51d664499bec25524ed7b6b2f51b72246d1fbde756669`  
		Last Modified: Wed, 02 Feb 2022 05:41:43 GMT  
		Size: 14.1 MB (14130296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735955845bdd39fb6bec511d39f6a3f91fdcd129d4673efceeeffb1fd71f543`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff820f8badf1b036673f852841f1f66f70fae3fdd930367b45e59622bee4be5`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c96f2aa98216b37f007ab4fc482783fbda6c1cb4f35278749e9d6cf21fb829`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe1b767832f1415d9e4b05ee726a113eb14f1c5ed1942644826961a7de2bb`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2225e04c87a6e2ef8f45524c9929cac9342e4c8b5c37109aa9a54421ddc280bd`  
		Last Modified: Wed, 02 Feb 2022 05:41:42 GMT  
		Size: 5.7 MB (5722410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:9050197bc9253da1306a219e5c38dc51ca41f3302d7888c9d05f94742e07a31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9a2d38540ca0b1dc0bb591b3487185110f0a07e783af525c5b86c15a28a0330d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113461123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284de8c381ad1b2a8189a13739a93a66dcf2fdab83b49943f9a97acf69e22b53`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 01 Feb 2022 02:32:58 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:32:58 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:32:58 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:32:59 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:32:59 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:32:59 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:32:59 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:33:00 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:33:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:33:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:33:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:33:10 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:33:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:33:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:33:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:33:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:33:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:33:20 GMT
USER 1001
# Tue, 01 Feb 2022 02:33:20 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:33:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:33:21 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:5e1dcd3d2744a39ecf8f1eb95e552c9539b5c0dc1494e733c3e3d623e4238921`  
		Last Modified: Tue, 01 Feb 2022 02:48:10 GMT  
		Size: 14.2 MB (14228744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264689484e10222b810a9835bd73fca46d470352f1409281894bd47289ca2de`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6458b29c6d007c2815431fed0e357875ba770119f91e2d3440ca2b65aaef9`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3707d42323ee4f32e04d5c800e6e75b4353c598aca35c595ce26cae4056a50`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff56ac88d4d78ee0500eed83f0de20125d9124f0b03822f6d043930dbe28face`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 10.6 KB (10644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3346f7e9502060f9168a88d25c05ce2e278b2295421bf05d3cf041302d5d43b`  
		Last Modified: Tue, 01 Feb 2022 02:48:06 GMT  
		Size: 2.5 MB (2497252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c1eb3c484964b48f70fbec011730ccc0b26dd7e2aa80cb32cc5eee87966659f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118895201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70835d223bdc357e86599ea85d6e089d4e92b58d9b17241361527eab2ea049c6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 12:30:02 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:30:06 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:30:09 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:30:12 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:30:17 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:30:20 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:30:22 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:30:23 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:30:25 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:34:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:34:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:34:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:34:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:34:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:34:26 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:34:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:34:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:34:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:34:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 12:34:56 GMT
USER 1001
# Wed, 02 Feb 2022 12:34:59 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:35:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:35:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:c629adcc50d21cebe396ee7b5026dd3d69f6029335c22b737b035812319c8c1e`  
		Last Modified: Wed, 02 Feb 2022 13:30:34 GMT  
		Size: 14.2 MB (14229389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59f56b86c301261a2a803a6d67d5174698150d320c3efe5e91e15509697dd8f`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21af9b4ba609b521be416c2a168614b33b85d6525b955a52af1489367c408e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc61794979abd71755b503170df22260137800fe704cc8234b27166c41cd762e`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2ae613b2a8041310d1994b1da58d012e404eb8c62eac7f661774f867b0895`  
		Last Modified: Wed, 02 Feb 2022 13:30:26 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbbe136d84c625633722280da81510ed9072b0456f4e6bc0a4c0c9047c9b141`  
		Last Modified: Wed, 02 Feb 2022 13:30:27 GMT  
		Size: 2.5 MB (2479493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:45b3564f7ef45bb9b96bfe3539da65b12a5d1749543910e9da075cf419fd689b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110581327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47c6d5b432741525623111529c7ab9af1e78b40da6dc471ef61af9cab008459`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 02 Feb 2022 05:09:54 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:54 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:55 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:55 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:55 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:55 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:55 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:10:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:10:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:10:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:10:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:10:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:10:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:10:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:10:15 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 02 Feb 2022 05:10:16 GMT
USER 1001
# Wed, 02 Feb 2022 05:10:16 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:10:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:10:16 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:c77602311a93edd5a58c83bbaf902ef7b03f2bee21e46360e6f3ad59f4045d23`  
		Last Modified: Wed, 02 Feb 2022 05:41:50 GMT  
		Size: 14.2 MB (14228938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab4fe7a0d81db18bac0038775ade0036f6ecd92c6573021d04cf632b6a183f`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee683ad878b74455936766919bde75a7517845a605dce5e6d20674d79b57b5b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f2fdd0c8a61e80f6ccf93143100796e740ab083de3f887522ab583411006a9`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc16640575440e02ab2598d69e93ffbc294b0bfe275d3eda05a77f2705a5d4b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787acc60dd91e6d838b87186e5d88fbde358467834865f7b7c3d87493f87442b`  
		Last Modified: Wed, 02 Feb 2022 05:41:48 GMT  
		Size: 2.5 MB (2500548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:32d04e4d823f6682982326360f3fa4caeeb5b235cd665ba05ef6403a6ef74cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:1523d1425988c2bd44ee54cfbe65d217eaa32202eed52014ba74294e22a59c68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.6 MB (465578785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e79631b682f29c4f03e4b297dc65a50ae4e26fda4d8564068ef547f39d9e982`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:26:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:27:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:27:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:21:48 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:21:48 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:28:52 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:28:52 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:28:53 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:28:53 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:28:53 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:28:53 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:29:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:29:19 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:29:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:29:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:29:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:29:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:29:22 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:29:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:29:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:29:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:29:33 GMT
USER 1001
# Tue, 25 Jan 2022 23:29:33 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:29:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:29:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 23:30:08 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 23:30:08 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 23:33:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 23:33:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 23:34:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c1a1f45083d49782e9c69cc2bb7cdc19bd099562f5f0aac114ad7bc7d8419`  
		Last Modified: Fri, 07 Jan 2022 03:28:57 GMT  
		Size: 3.0 MB (2960369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee93795afea436bc51adcf292fea2b49d5a4051ff33ab0cc16357105957cea`  
		Last Modified: Fri, 07 Jan 2022 03:29:06 GMT  
		Size: 128.7 MB (128726677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684cbf0832df4654ac666b7af4422d156c1e5ebc781c84a861b9876fd6719ad9`  
		Last Modified: Tue, 25 Jan 2022 23:40:12 GMT  
		Size: 14.1 MB (14130816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdd64484cfa06e57ebfba3acc22e4ec6779557b52d55a3fafad7a4ed4eae8e9`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95128698b2f7eb1a6e3dd47b30695b0ebac941fce5b5790f2b1b49987ec29a5a`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16d0044e066e31dbad560d64450bf3b182e65d9f913823b5066aa3c79c39c0c`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17802f8569a2d6741632ab087d9461ff3aacb49e8b260ad622e79cd042127bfc`  
		Last Modified: Tue, 25 Jan 2022 23:40:08 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7a4b18294b82e0fd276930e5f828a812c3101ffbced931e44c4a359697634`  
		Last Modified: Tue, 25 Jan 2022 23:40:10 GMT  
		Size: 5.7 MB (5655523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50e52c6aa148d7c7b338b00e0c24b0d4a815d021bfb941913df0b0851d5c4f1`  
		Last Modified: Tue, 25 Jan 2022 23:40:52 GMT  
		Size: 271.1 MB (271128666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35be19483cac5f6a010f8262cb95240db20619ec93bdf32cbfaf7b36d4c5807`  
		Last Modified: Tue, 25 Jan 2022 23:40:39 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b92982762035daabfc5fb8d0bff64015300723be82b825ff85c93af44c9968`  
		Last Modified: Tue, 25 Jan 2022 23:40:42 GMT  
		Size: 16.2 MB (16249449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:90866fcb374315d224ccd6f53dd26b2166e79bda95726a25dc3373fea2a25279
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466059188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f21f2cb7cf9c1516aa78f39e4414381affc89efb0f819cfbd4f727f0097e35f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:01:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 06:01:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:01:57 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 06:02:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 06:03:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:25:21 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:25:23 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:25:26 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 12:25:29 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 12:25:31 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 12:25:32 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 12:25:36 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 12:25:37 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 12:25:40 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 12:28:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 12:28:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 12:28:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 12:28:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 12:28:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 12:28:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 12:28:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 12:29:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 12:29:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 12:29:30 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 12:29:32 GMT
USER 1001
# Wed, 02 Feb 2022 12:29:35 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 12:29:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 12:29:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 12:35:15 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 12:35:17 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 12:40:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 12:40:17 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 12:41:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e519c40c78b488d71991dd0054bffe8260611286580cb61463ffb1d4b81bb2`  
		Last Modified: Wed, 02 Feb 2022 06:05:57 GMT  
		Size: 3.1 MB (3081867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc06ac8fcfae7601e6713eb3490af9d0691a2919c0470e01afd618fff11403`  
		Last Modified: Wed, 02 Feb 2022 06:06:11 GMT  
		Size: 128.3 MB (128256175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bdd8addeaf2c0b6bb30d08a19e51130187d8e5e24e046eced8cf481f611bf8`  
		Last Modified: Wed, 02 Feb 2022 13:30:18 GMT  
		Size: 14.1 MB (14130794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4224b13f14b349ab121fc8921d706e872baf263faf40b5569a0be3a90dc641`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9540b5678c1e636d2cddfa7fb7e893576b7b68d50b52dfa5aace97d09abf9c08`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426b46c2de6c5cab17c57667b78bc99a62b010696889b3a733865e5fa307038b`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c0353910905dbcb8e90ac0424838bad1bc1490244ec658b67125e339bb37e5`  
		Last Modified: Wed, 02 Feb 2022 13:30:06 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b548213c4a4358f74e22dbc35c05cfbf76610870900e8cb282aefe4d318c9b7`  
		Last Modified: Wed, 02 Feb 2022 13:30:08 GMT  
		Size: 5.3 MB (5255386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a339184bb89b8167f43d5fc1a94213349bc819c866d54b59432d8d6a7cdc2`  
		Last Modified: Wed, 02 Feb 2022 13:31:48 GMT  
		Size: 271.1 MB (271129407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d05420f0f7365a419a31f6712d794d606bcf351ece8f9a04f38bb297c5496de`  
		Last Modified: Wed, 02 Feb 2022 13:30:43 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acb9725035238f7f7d7fee9a0a0032aac45f265c569375e104f1bf01a6b45a`  
		Last Modified: Wed, 02 Feb 2022 13:30:46 GMT  
		Size: 13.7 MB (13745624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:21d37155d493324cc388d37767a473ed148955b7c9a9ed7cd65305130e60ed8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460722956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4898ad2a7e8479a21d4f806f585f787645a90d7eed83919e40a7ef466e4ba2d7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:03 GMT
ADD file:3fe2ce9d5d8932ed39dc2c73abff4b15e244fb1e7eb456de0a05df07ede3bf39 in / 
# Wed, 02 Feb 2022 01:42:07 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:39:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 02 Feb 2022 02:39:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:39:35 GMT
ENV JAVA_VERSION=8.0.7.0
# Wed, 02 Feb 2022 02:40:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 02 Feb 2022 02:40:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:27 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:09:27 GMT
ARG OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:27 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Wed, 02 Feb 2022 05:09:28 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Wed, 02 Feb 2022 05:09:28 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 02 Feb 2022 05:09:28 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Wed, 02 Feb 2022 05:09:28 GMT
ARG LIBERTY_URL
# Wed, 02 Feb 2022 05:09:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 02 Feb 2022 05:09:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:09:40 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:09:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Wed, 02 Feb 2022 05:09:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 02 Feb 2022 05:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 02 Feb 2022 05:09:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 02 Feb 2022 05:09:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 02 Feb 2022 05:09:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 02 Feb 2022 05:09:48 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 02 Feb 2022 05:09:48 GMT
USER 1001
# Wed, 02 Feb 2022 05:09:48 GMT
EXPOSE 9080 9443
# Wed, 02 Feb 2022 05:09:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 02 Feb 2022 05:09:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 02 Feb 2022 05:10:23 GMT
ARG VERBOSE=false
# Wed, 02 Feb 2022 05:10:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 02 Feb 2022 05:14:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 02 Feb 2022 05:14:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 02 Feb 2022 05:15:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:cf002da3924024b39105dcc613288421b394e45e04d7a3c245ce5dcaf544dd98`  
		Last Modified: Wed, 02 Feb 2022 01:43:50 GMT  
		Size: 25.4 MB (25364307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bcdb503991176c9486c76e56946053a4588fc20649c5465c056a465c592dee`  
		Last Modified: Wed, 02 Feb 2022 02:42:23 GMT  
		Size: 2.7 MB (2676856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df62e0db73c50d4083fae4ee06f49a970987b3ca04733d34734617f91cfccf`  
		Last Modified: Wed, 02 Feb 2022 02:42:32 GMT  
		Size: 125.7 MB (125737326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8d99305c3aacb5d4b51d664499bec25524ed7b6b2f51b72246d1fbde756669`  
		Last Modified: Wed, 02 Feb 2022 05:41:43 GMT  
		Size: 14.1 MB (14130296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735955845bdd39fb6bec511d39f6a3f91fdcd129d4673efceeeffb1fd71f543`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff820f8badf1b036673f852841f1f66f70fae3fdd930367b45e59622bee4be5`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c96f2aa98216b37f007ab4fc482783fbda6c1cb4f35278749e9d6cf21fb829`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febfe1b767832f1415d9e4b05ee726a113eb14f1c5ed1942644826961a7de2bb`  
		Last Modified: Wed, 02 Feb 2022 05:41:41 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2225e04c87a6e2ef8f45524c9929cac9342e4c8b5c37109aa9a54421ddc280bd`  
		Last Modified: Wed, 02 Feb 2022 05:41:42 GMT  
		Size: 5.7 MB (5722410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba19544da9e3e1e528ba844c095f75be212ea1ef20cf6f9930b1dd6722d0df5d`  
		Last Modified: Wed, 02 Feb 2022 05:42:07 GMT  
		Size: 271.1 MB (271128976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf5b3e381e121e19f39fa92edec3c96d222f34fb75effb09082f1ddad0ac796`  
		Last Modified: Wed, 02 Feb 2022 05:41:56 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c8b74b60a36baf6ce0e1ee249c6693f04d466539db0029b0a623a6bc802def`  
		Last Modified: Wed, 02 Feb 2022 05:41:58 GMT  
		Size: 15.9 MB (15940538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
